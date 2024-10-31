---
Topic: Programming Fundamentals
tags:
  - Academia
  - School
  - Computer-Science
  - Programming
  - Revision
aliases:
  - Switch
  - Selection
  - CASE SELECT
  - SWITCH
Links:
  - "[[Switch Statements|Selection]]"
  - "[[Programming Loops]]"
---
# Switch Statements: 


> [!info] What are they? 
> <mark class="hltr-blue">Switch statements are another form of selection, like [[IF Selection]].</mark> However, instead of checking if a statement is true or false: <mark class="hltr-green">switch statements check for specific values in a variable,</mark> and are incredibly versatile. They are typically used when you want a program to perform different actions for different values of the same variable. 

<mark class="hltr-red">In Python, there is no official "switch" statement like in some other programming languages</mark> such as Java or C. However, we can achieve similar functionality using other control flow structures, such as "if", "elif", and "else". Here's an example that demonstrates how to implement a switch-like structure in Python:

```python
def switch_example(value):
    if value == 1:
        print("Value is 1")
    elif value == 2:
        print("Value is 2")
    elif value == 3:
        print("Value is 3")
    else:
        print("Value is not 1, 2, or 3")

# Example usage
switch_example(1)
switch_example(2)
switch_example(3)
switch_example(4)
```

**Switch statements have a very similar structure to [Nested IF](IF%20Selection.md#Nested%20IF) statements**

In programming, sometimes we need to repeat code: this is where [[Programming Loops]] come into place, they are iteration statements that repeat a part of a program. 