---
layout: post
title:  "Learn Python 3 the Hard Way: Exercise 1 - 3 で学んだこと"
---

[Learn Python 3 the Hard Way](https://learnpythonthehardway.org/)の「Exercise 1 - 3」で学んだことのまとめです。

Pythonの世界に入る方法

```
python3.6
```

Pythonの世界から出る方法

```
quit()
```

## Exercise 1: A Good First Program

```python
print("Hello world!")
print("Hello Again")
print("I like typing this.")
print("This is fun.")
print('Yay! Printing.')
print("I'd much rather you 'not'.")
print('I "said" you do not touch this.')
```

実行方法:

```
python3.6 chapter1/ex1.py
```

## Exercise 2: Comments and Pound Characters

```python
# A comment, this is so you can read your program later.
# Anything after the # is ignored by python.

print("I could have code like this.") # and the comment after this is ignored

# You can also use a comment to "disable" or comment out code:
# print("This won't run.")

print("This will run." )

print("Hi # there")
```

実行方法:

```
python3.6 chapter2/ex2.py
```

## Exercise 3: Numbers and Math

```python
print("I will now count my chickens:")

# Hens 30.0
print("Hens", 25 + 30 / 6)

# Roosters 97
print("Roosters", 100 - 25 * 3 % 4)

print("Now I will count the eggs:")

# 6.75
print(3 + 2 + 1 - 5 + 4 % 2 - 1 / 4 + 6)

print("Is it true that 3 + 2 < 5 - 7?")

# False
print(3 + 2 < 5 - 7)

# what is 3 + 2? 5
print("what is 3 + 2?", 3 + 2)

# what is 5-7? -2
print("what is 5-7?", 5 - 7)

print("Oh, that's why it's False.")

print("How about some more.")

# Is it greater? True
print("Is it greater?", 5 > -2)

# Is it greater or equal? True
print("Is it greater or equal?", 5 >= -2)

# Is it less or equal? False
print("Is it less or equal?", 5 <= -2)
```

実行方法:

```
python3.6 chapter3/ex3.py
```
