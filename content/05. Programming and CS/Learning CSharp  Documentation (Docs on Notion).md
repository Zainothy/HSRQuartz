---
tags:
  - Csharp
  - Computer-Science
  - favorite
Topic: Programming
Completed: 
Links:
  - "[[Understanding UI Design]]"
---

## Goals: 

- **Understand advanced C# Syntax**
- **Learn UI Design Essentials [[Understanding UI Design]]**

## Achievements: 

- **Understood basic namespace structure and method args**
- **Understood Data Types and Variables**
## Struggles: 

- **Understanding the manual and statically typed nature of the language**
- **Getting used to the different debugging methods and IDE systems**
### Courses used: 
https://www.w3schools.com/cs/
https://learn.microsoft.com/en-us/dotnet/csharp/

## References :
1. The Calculator code is on the notion page: 

### Notion Page: 
> https://www.notion.so/Learning-C-fee1a4d943ae44479c7a087b10cef0e7?pvs=4



## Useful Info: 


### Data Types & Type Casting:

**The advantage of explicit casting is that it allows you to convert a larger type to a smaller type, or a base class to a derived class, when the conversion is not guaranteed to succeed or may cause data loss. Explicit casting requires a cast expression, such as `(int)x` or `x as int`, to indicate the desired type. Implicit casting is automatic and does not need a cast expression, but it only works when the conversion is safe and no data will be lost, such as from a smaller type to a larger type, or a derived class to a base class. Type conversion is a general term that includes both implicit and explicit casting, as well as other ways of changing the type of a value, such as using methods like `Convert.ToInt32(x)` or `int.Parse(x)`.**

## Mathematics:

- **The `Math.Max(_x_,_y_)` method can be used to find the highest value of _x_ and _y_ 
- **The `Math.Min(_x_,_y_)` method can be used to find the lowest value of of _x_ and _y_ 
- **The `Math.Sqrt(_x_)` method returns the square root of _x_
- **The `Math.Abs(_x_)` method returns the absolute (positive) value of _x_
- **`Math.Round()` rounds a number to the nearest whole number


## Strings: 

**Strings are used for storing text.
A `string` variable has a set if characters:**

```csharp
string greeting = "Hello";
string greeting2 = "Nice to meet you!";
```

**A string in C# is actually an object, which contain properties and methods that can perform certain operations on strings. For example, the length of a string can be found with the `Length` property:**

```csharp
string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
Console.WriteLine("The length of the txt string is: " + txt.Length);
```

