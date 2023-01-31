# Looping

## Learning Goals

- Explain a loop.
- Write a `while` loop.

## Introduction

We want to write a program to print all the numbers from `1` to `5`. Here’s a
possible solution:

```python
print(1)
print(2)
print(3)
print(4)
print(5)
```

That is a lot of duplicated code. Imagine if we had to print all the numbers up
to `100` or `1000` or a million! How can we make it easier to perform repetitive
tasks?

Well, the great news is that programming languages usually have features to make
this easier. One of those features is called a `loop`. A `loop` is a way to
perform operations until a condition is satisfied.

## A `while` Loop

Here’s the general structure of a `while` loop:

```python
while (condition is True):
	# do something
```

The simplest form of this structure is the following:

```python
# DO NOT RUN THIS CODE
while (True):
	print("Hello")
```

The above code is telling the computer to display the value `"Hello"` in the
console until the condition is `False`. There is no logic in the code that
instructs the computer to stop.

### The `break` Statement

The `break` statement is used to stop a loop.

```python
while (True):
	print("Hello")
	break
```

Output:

```python
Hello
```

- The program starts the `while` loop.
- The condition is evaluated to `True`.
- The `print` function is invoked and displays `Hello` in the console.
- The loop immediately stops once the `break` statement is executed.

### Printing Numbers with a Loop

We can use the `while` loop and the `break` statement to write a program to
print all the values from a starting value up to an ending value:

```python
current = 1
end = 4

while (True):
  if (current == end):
    break
  print(current)
  current = current + 1

print(current)
```

### A Common Loop Format

You may see the following format being used in a lot of codebases:

```python
i = 0
end = 4

while (i < end):
	print(i)
	i = i + 1

print("The value of i is " + str(i))
```

Output:

```python
0
1
2
3
The value of i is 4
```

Use [this visualizer](https://pythontutor.com/python-debugger.html) to observe
how this code is run by Python. The variable `i` is a common way to represent
loop variables, i.e., variables that are only used inside of a loop.

## Conclusion

In this lesson, we have learned how to use loops to make writing repetitive code
a lot easier. You will be writing loops all the time when you build programs, so
be sure to practice writing a bunch of them!
