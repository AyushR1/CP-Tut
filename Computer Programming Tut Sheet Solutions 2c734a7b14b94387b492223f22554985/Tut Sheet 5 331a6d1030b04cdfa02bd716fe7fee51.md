# Tut. Sheet 5

Solutions @Ayush Rathore 

# 

Q2. Getting multiple outputs from functions on arrays like bounds().

Q3. Display function:

1. String
2. Number
3. Variable value
4. Without parentheses string, numeric and variables

Q4. Clearing the command window and workspace.

Q5. Plot functions:

1. 2-D
2. 3-D
3. Multiple plots on a single graph
4. Multiple plots on tiled on single figure window
5. Title of graph and axes
6. Color and symbol for plot

Q6. Loops to generate arithmetic and geometric series.

Q7. if-else-else if example.

Q8. Multiple lines input:

1. Long mathematical expression
2. Long string
3. Multiple matrix values

Q9. Check whether a variable exists and if yes delete it from workspace.

Q10. Compact the outputs appearing in command window.

Q1. Examples for functions like max, min etc. on arrays.

A1. Examples of functions such as **`max`**, **`min`**, etc. on arrays in MATLAB can be:

```
A = [1, 2, 3, 4, 5];
maximum = max(A); % maximum = 5
minimum = min(A); % minimum = 1
```

 Examples of functions such as **`max`**, **`min`**, etc. on arrays in MATLAB ask for examples of how to use functions like **`max`** and **`min`** on arrays in MATLAB. These functions are used to find the maximum and minimum values in an array respectively.

A2. To get multiple outputs from functions on arrays like **`bounds()`**, one can assign the outputs to multiple variables:

A2. To get multiple outputs from functions on arrays like **`bounds()`**, one can assign the outputs to multiple variables:

```
[minimum, maximum] = bounds(A);

```

A3. To display values in MATLAB:

A3. To display values in MATLAB:

```
string = 'Hello World!';
number = 42;
variable_value = maximum;
disp(string); % displays "Hello World!"
disp(number); % displays 42
disp(variable_value); % displays 5

```

Without parentheses:

```
disp string; % displays "Hello World!"
disp number; % displays 42
disp variable_value; % displays 5
```

A4. To clear the command window in MATLAB:

```
clc;
```

To clear the workspace in MATLAB:

```
clear;
```

A5. Plot functions in MATLAB:
2-D plot:

```
x = 0:0.1:10;
y = sin(x);
plot(x, y);

```

3-D plot:

```
[X, Y] = meshgrid(-2:.2:2);
Z = X .* exp(-X.^2 - Y.^2);
surf(X, Y, Z);

```

Multiple plots on a single graph:

```
x = 0:0.1:10;
y1 = sin(x);
y2 = cos(x);
plot(x, y1, x, y2);

```

Multiple plots tiled on single figure window:

```
subplot(2,1,1);
plot(x, y1);
subplot(2,1,2);
plot(x, y2);

```

Title of graph and axes:

```
x = 0:0.1:10;
y = sin(x);
plot(x, y);
title('Sine Function');
xlabel('x');
ylabel('y');

```

Color and symbol for plot:

```
x = 0:0.1:10;
y = sin(x);
plot(x, y, '--r');

```

A6. Loops to generate arithmetic and geometric series in MATLAB:
Arithmetic series:

```

n = 10;
a = 2;
d = 3;
sum = 0;
for i = 1:n
    sum = sum + a;
    a = a + d;
end
disp(sum);

```

Geometric series:

```
n = 10;
a = 2;
r = 3;
sum = 0;
for i = 1:n
    sum = sum + a;
    a = a * r;
end
disp(sum);

```

A7. An **`if-else-elseif`** example in MATLAB:

```matlab
x = 42;
if x > 0
    disp('Positive');
elseif x < 0
    disp('Negative');
else
    disp('Zero');

```

A1. Examples of functions such as **`max`**, **`min`**, etc. on arrays in MATLAB asks for examples of how to use functions like **`max`** and **`min`** on arrays in MATLAB. These functions are used to find the maximum and minimum values in an array respectively.

A2. Getting multiple outputs from functions on arrays like **`bounds()`** asks for a method to get multiple outputs from a function in MATLAB that operates on arrays, such as the **`bounds()`** function.

A3. Display function asks for examples of how to display different types of values in MATLAB, such as strings, numbers, and variable values, both with and without parentheses.

A4. Clearing the command window and workspace asks for examples of how to clear the command window and the workspace in MATLAB.

A5. Plot functions asks for examples of different types of plot functions in MATLAB, including 2-D plots, 3-D plots, multiple plots on a single graph, multiple plots tiled on a single figure window, title of graph and axes, and color and symbol for plot.

A6. Loops to generate arithmetic and geometric series asks for examples of how to generate arithmetic and geometric series using loops in MATLAB.

A7. if-else-else if example asks for an example of how to use the **`if-else-elseif`** control statement in MATLAB.

A8. Multiple lines input asks for examples of how to input multiple lines of data in MATLAB, including a long mathematical expression, a long string, and multiple matrix values.

A9. Check whether a variable exists and if yes delete it from workspace asks for a method to check if a variable exists in the workspace and if it exists, delete it.

A10. Compact the outputs appearing in the command window asks for a method to compact the outputs that appear in the command window in MATLAB.

A8. Multiple lines input in MATLAB:
Long mathematical expression:

```

expression = (2 + 3) * (4 + 5) / (6 + 7) - (8 + 9);
disp(expression);

```

Long string:

```
string = ['This is a long string ' ...
         'which is split into multiple lines ' ...
         'for better readability'];
disp(string);

```

Multiple matrix values:

```
A = [1 2 3; 4 5 6; 7 8 9];
B = [9 8 7; 6 5 4; 3 2 1];
C = [A B];
disp(C);

```

A9. To check whether a variable exists in the workspace and delete it:

heck whether a variable exists and if yes delete it from workspace asks for a method to check if a variable exists in the workspace and if it exists, delete it

```
if exist('variable_value', 'var') == 1
    clear variable_value;
end

```

A10. To compact the outputs appearing in the command window in MATLAB:

A10. Compact the outputs appearing in the command window asks for a method to compact the outputs that appear in the command window in MATLAB

```
format compact;

```

A2. Getting multiple outputs from functions on arrays like **`bounds()`** asks for a method to get multiple outputs from a function in MATLAB that operates on arrays, such as the **`bounds()`** function.

A3. Display function asks for examples of how to display different types of values in MATLAB, such as strings, numbers, and variable values, both with and without parentheses.

A4. Clearing the command window and workspace asks for examples of how to clear the command window and the workspace in MATLAB.

A5. Plot functions asks for examples of different types of plot functions in MATLAB, including 2-D plots, 3-D plots, multiple plots on a single graph, multiple plots tiled on a single figure window, title of graph and axes, and color and symbol for plot.

A6. Loops to generate arithmetic and geometric series asks for examples of how to generate arithmetic and geometric series using loops in MATLAB.

A7. if-else-else if example asks for an example of how to use the **`if-else-elseif`** control statement in MATLAB.

A8. Multiple lines input asks for examples of how to input multiple lines of data in MATLAB, including a long mathematical expression, a long string, and multiple matrix values.