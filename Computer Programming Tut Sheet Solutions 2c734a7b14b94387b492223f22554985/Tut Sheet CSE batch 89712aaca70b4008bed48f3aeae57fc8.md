# Tut Sheet CSE batch

@Ayush Rathore

Star the repo if it helped!

Respective PDFs attached.

# 1. Report the output or error(s), if any, of the following programs/code snippets.

# a.

```cpp
#include <stdio.h>
int i = 5;
int fun(){
i++;
return 1;
}
int main(){
printf("%d", fun()*i);
}
```

output :- 6

# b.

```cpp
#include <stdio.h>
int i = 5;
int fun(){
printf("%d\n",i);
i++;
return 1;
}
int main(){
printf("%d", fun()*i + ++i);
}
```

5

13

# c.

```cpp
#include <stdio.h>
int i = 5;
int fun(){
printf("%d\n",i);
i++;
return 1;
}
int main(){
printf("%d", fun()*i + i++);
}
```

5

12

# d.

```cpp
#include <stdio.h>
int fun();
int fun1();
int i = 5;
int main(){
printf("%d", fun()*i);
}
void fun1(){
i--;
}
int fun(){
printf("%d\n",i);
i++;
return 1;
}
```

wrong void 

5

6

# e.

```cpp
#include <stdio.h>
int fun();
void fun1();
int fun2();
int i = 5;
int fun2(){
printf("%d", fun()*i);
}
void fun1(){
i--;
}
int fun(){
printf("%d\n",i);
i++;
return 1;
}
```

wrong no int main

if put main 

then 

5

5

6

# f.

```cpp
#include <stdio.h>
int i =0;
int
fun ()
{
  printf ("%d\n", i);
  i++;
  return 1;
}

int
main ()
{
  int i = 5;
  printf ("%d", fun () * i + ++i);
}
```

not correct i not defined 

scope

0 

11

# g.

```cpp
#include <stdio.h>
int fun(int k){
printf("%d\n",i);
i++;
return 1;
}
int main(){
int i = 5;
printf("%d", fun()*i + ++i);
}
```

I underlared change k to i

pass i

5

11

# h.

```cpp
#include <stdio.h>
int fun(int k){
printf("%d\n",k);
k++;
return 1;
}
int main(){
int i = 5;
printf("%d", fun(i)*i + ++i);
}
```

5

11

# i.

```cpp
#include <stdio.h>
int printf(char s, int i, int j){
printf("%c %d %d\n",s, i, j);
}
int fun(int k){
printf("%d\n",k);
k++;
return 1;
}
int main(){
int i = 5;
printf("%d", fun(i)*i + ++i);
}
```

printf declared multiple times

5

11

# j.

```cpp
int, double fun(int k){
k++;
return k;
}
```

change double,int to int

# k.

```cpp
for(int i = 10; i < 100; i += 10, i -= 10){
printf("%d\n", i);
}
```

Infintte loop

# l.

```cpp
for(int i = 10; i < 100; i += 10){
printf("%d\n", i);
break;
}
```

10

# m.

```cpp
#include <stdio.h>
void fun(int *k){
(*k)++;
}
int main(){
int i = 5;
fun(&i);
printf("%d",i);
}
```

6

# n.

```cpp
int main( ){
int i = 5, j = 2;
fun(&i, &j );
printf ("\n%d %d", i, j);
}
void fun( int *i, int *j){
*i = *i * *i;
*j = *j * *j;
}
```

25 4

# o.

```cpp
#include <stdio.h>
int main (){
int i = 35, *z ;
z = function ( &i ) ;
printf ( "\n%d", z ) ;
}
int function ( int *m ){
return ( m + 2 );
}
```

adreess of m + 2

# 2. Write a recursive function to compute the factorial of a given number.

```cpp
int factorial(int n)  
{  
  if (n == 0)  
    return 1;  
  else  
    return(n * factorial(n-1));  
}
```

# 3. Write a recursive function to compute the fibonacci series up to a given number of terms.

```cpp
int main()
{
   int n, i = 0;
 
   scanf("%d",&n);
 
   for (int c = 1 ; c <= n ; c++ )
   {
      printf("%d\n", Fibonacci(i));
      i++; 
   }
 
   return 0;
}
 
int Fibonacci(int n)
{
   if ( n == 0 )
      return 0;
   else if ( n == 1 )
      return 1;
   else
      return ( Fibonacci(n-1) + Fibonacci(n-2) );
}
```

0, 1, 1, 2, 3, 5, 8, 13, 21,

### extra knowledge using dynamic programming (memoization)

```cpp
int fib (int n){
        vector <int> dp(n+1,-1);
        return dp_fib(n, dp);
    }
    int dp_fib(int n,vector<int> &dp) {
        if(n<=1)
            return n;
        
        if(dp[n]!=-1) return dp[n];
        
        return dp[n]=dp_fib(n-1,dp)+dp_fib(n-2,dp);
       
    }

```

# 4. Write a recursive function to compute the sum of first n (user input) prime numbers.

Recursive summation of n prime

```cpp
bool isPrime(int n, int i = 2)
{
    if (n <= 2)
        return (n == 2) ? true : false;
    if (n % i == 0)
        return false;
    if (i * i > n)
        return true;

    return isPrime(n, i + 1);
}

while(1) {
      j++;
      if(isprime(j)) {
         sum += j;
         i++;
      }
      if(i == n) {
         break;
      }
   }
```

extra knowledge sieve of eratosthenes