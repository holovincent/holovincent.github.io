---
layout: post
title:  "Code Complete Notes: Chapter 12"
date: 2016-07-26
categories: cpp
tags:  Code-Complete
---

* content
{:toc}


### Chapter 12: Fundamental Data Types

#### 12.1: Numbers in General

* Replace **"magic numbers"** with named constant can make your code more readable and changes reliable and easy 
* Make type conversion obvious and avoid mixed-type comparisons

#### 12.2: Integers

* Check for integer division and reorder the expression to put divisions the end
* Check for integer overflow especially intermediate resutls overflow

#### 12.3: Floating-Point Numbers

* Avoid additions and subtractions on numbers that have greatly different magnitudes
* Sort the numbers before add a sequence of numbers that contains huge differences and add them starting with the smallest values
* Replace equality comparisons with a accuracy check
* Change from floating-point to integer variables by multipling constant times to deal with rounding errors 

#### 12.4: Characters and Strings

* Use Unicode if need multiple language support
* To avoid endless strings in C, initialize strings to null

#### 12.6: Enumerated Types

* Enumerated types are generally used when you know all the possible values of a variable and want to express them in English words
* Enumerated types can increase readability, easier modifications
* Enumerated types can be a richer alternative to boolean variables

#### 12.7: Named Constant

* Named constant is a way of **"parameterizing"** the program

#### 12.8: Arrays

* Arrays are the simplest and most common type of **structured** data
* Make sure all array indexed are within the bounds of the array
* Consider using container instead of arrays

#### 12.9: Creating Your Own Types

* Programmer-defined types can make modifications easier, avoid excessive information distribution, and increase reliability
* Create types with functionally orientated names and avoid creating type names that refer to predefined types like BigInteger