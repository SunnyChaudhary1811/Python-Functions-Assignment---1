Question 1: 

Origin: Built-in functions come pre-defined with the Python language, while user-defined functions are created by programmers as needed.
Availability: Built-in functions are available without any additional work, while user-defined functions must be defined in your code before they can be used.
Purpose: Built-in functions cover common operations and tasks, whereas user-defined functions allow you to encapsulate custom logic and functionality.
Customization: You have control over the implementation and behavior of user-defined functions, but built-in functions are fixed and cannot be modified.


```python
#builtin
my_list = [1, 2, 3, 4, 5]
length = len(my_list)
print(length)  

```

    5
    


```python
#userdefined
def square(x):
    return x * x

result = square(5)
print(result)  

```

    25
    

Question 2:

 you can pass arguments to a function when you call it. Arguments are values that you provide to the function so that it can perform its operations using those values.
 
 In positional arguments, the order of the arguments matters. The first argument you provide corresponds to the first parameter, the second argument to the second parameter, and so on.
In keyword arguments, you explicitly specify which argument corresponds to which parameter using the parameter name. This allows for more clarity, especially when a function has many parameters.
You can use both positional and keyword arguments in the same function call, but positional arguments must come before keyword arguments.

Question 3:

The return statement in a function serves the purpose of exiting the function and returning a value back to the caller. When a return statement is encountered in a function, the function's execution immediately stops, and the value specified in the return statement is sent back to the caller.

A function can indeed have multiple return statements. However, once a return statement is executed, the function's execution stops, and the value from that return statement is returned. This means that only one return statement will be executed for a single function call, even if there are multiple return statements in the function's code. This makes sense, as the function should provide a single output for a given set of inputs.


```python
def compare_numbers(a, b):
    if a > b:
        return f"{a} is greater than {b}"
    elif a < b:
        return f"{a} is less than {b}"
    else:
        return f"{a} and {b} are equal"

result1 = compare_numbers(5, 3)
print(result1)  

result2 = compare_numbers(2, 7)
print(result2)  

result3 = compare_numbers(4, 4)
print(result3)  

```

    5 is greater than 3
    2 is less than 7
    4 and 4 are equal
    

Question 4:

a lambda function is a small, anonymous function that can have any number of arguments but can only have one expression. Lambda functions are often used for simple operations that can be defined in a single line of code. They are sometimes referred to as "anonymous functions" because they don't require a formal def statement to create them, and they don't have a name associated with them.


```python
add = lambda x, y: x + y
result = add(3, 5)
print(result)  

```

    8
    

Question 5:

Scope in Python:
Scope defines where variables can be accessed. There are two types of scope:

Local Scope: Variables defined within a function are only accessible inside that function.
Global Scope: Variables defined outside any function are accessible throughout the entire program.
Local variables take precedence over global variables with the same name within their respective scopes. Understanding scope helps avoid conflicts and manage variable visibility.

Question 6:

To return multiple values from a Python function:

Pack the values into a tuple, list, or dictionary.
Use the return statement followed by the data structure.


```python
def multiple_values():
    x = 10
    y = 20
    z = 30
    return x, y, z

result = multiple_values()
print(result)  

```

    (10, 20, 30)
    

Question 7:

arguments are passed by object reference. It's neither exactly "pass by value" nor "pass by reference."

Immutable objects (like numbers, strings) behave somewhat like "pass by value."
Mutable objects (like lists, dictionaries) behave somewhat like "pass by reference."
This behavior is due to how objects are shared and modified, offering a more flexible approach than traditional pass-by-value or pass-by-reference concepts.

Question 8:


```python
import math

def perform_operations(value):
    # Logarithmic function (log x)
    log_result = math.log(value)
    
    # Exponential function (exp(x))
    exp_result = math.exp(value)
    
    # Power function with base 2 (2^x)
    power_result = math.pow(2, value)
    
    # Square root
    sqrt_result = math.sqrt(value)
    
    return log_result, exp_result, power_result, sqrt_result

# Test the function
input_value = 4.0
log_result, exp_result, power_result, sqrt_result = perform_operations(input_value)

print(f"Logarithmic function: log({input_value}) = {log_result}")
print(f"Exponential function: exp({input_value}) = {exp_result}")
print(f"Power function with base 2: 2^{input_value} = {power_result}")
print(f"Square root: sqrt({input_value}) = {sqrt_result}")

```

    Logarithmic function: log(4.0) = 1.3862943611198906
    Exponential function: exp(4.0) = 54.598150033144236
    Power function with base 2: 2^4.0 = 16.0
    Square root: sqrt(4.0) = 2.0
    

Question 9:


```python
def extract_first_last_name(full_name):
    names = full_name.split()  
    first_name = names[0]
    last_name = names[-1]  
    
    return first_name, last_name


full_name = "John Doe"
first_name, last_name = extract_first_last_name(full_name)

print("First Name:", first_name)
print("Last Name:", last_name)

```

    First Name: John
    Last Name: Doe
    


```python

```
