# Exercise 1 - Character Input (*) #

Keywords: *input*, *strings*, *types*, *int*
[Original post](https://www.practicepython.org/exercise/2014/01/29/01-character-input.html).
[Original solution](https://www.practicepython.org/solution/2014/02/05/01-character-input-solutions.html).

Copyright CC-BY-4.0 Michele Pratusevich.

Content has been modified, with changes to style and shortening of content for the purpose of creating a consise, condensed version of the exercise prompt.

***

## Challenge ##

### Tasks ###

Create a program that **asks the user to enter their name and their age** and **prints out a message addressed to them that tells them the year that they will turn 100 years old**.

### Extras ###

1. Add on to the previous program by asking the user for another number and printing out that many copies of the previous message.
2. Print out that many copies of the previous message on separate lines.

### Hints ###

- [Order of operations](http://www.mathsisfun.com/operation-order-pemdas.html) exists in Python.
- The string `\n` is the same as pressing the `ENTER` button.

***

## Discussion ##

This exercise covers the following concepts:

- Getting user input.
- Manipulation of strings.

### User Input in Python ###

The `input()` command can be used to get user input in Python 3. The results should be stored in a variable. The result from a user will be a string - even if they enter a number.

For example,

```python
name = input("Give me your name: ")
print("Your name is " + name)
```

The above will output the following:

```bash
>>> Give me your name: Example
Your name is Example
```

After `input()` is called, the program will wait until the user presses the `ENTER` key. The program will not continue until this happens.

### String Manipulation in Python ###

The `input()` function returns a string. There are a couple of things that you can do with strings in Python; these are just a few examples.

#### Casting into Integers ####

A string that contains a number can be cast into an integer using the `int()` function:

```python
age = input("Enter your age: ")
age = int(age)
```

This operation can be condensed into one line to make your code more compact:

```python
age = int(input("Enter your age: "))
```

In both cases, age will hold an integer variable after casting. You can turn integers into strings by using the `str()` function instead.

#### String Concatenation ####

You can **add** strings together in Python. This is known as string **concatenation**. You simply need two string objects:

```python
print("Were" + "wolf")
print("Door" + "man")
print("4" + "chan")
print(str(4) + "chan")
```

The above would output:

```bash
Werewolf
Doorman
4chan
4chan
```

You can also **multiply** strings:

```python
print(4 * "test")
```

The above would ouput:

```bash
testtesttesttest
```

It is important to note that you cannot multiply or divide a string by another string. Since the concept of multiplying a string by another string is not well-defined, it would be hard to create functionality for it. However, it makes sense in a way to specify multiplying a string by a number - just repeat that string that number of times.

***

View the solution for this exercise here. (Solution pending).

***

Return to the [table of contents](https://github.com/rimij405/praticepython-solutions/blob/master/table-of-contents.md).