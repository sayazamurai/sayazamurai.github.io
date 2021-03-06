---
layout: post
title:  "Learn Python 3 the Hard Way: Exercise 4 - 6で学んだこと"
---

[Learn Python 3 the Hard Way](https://learnpythonthehardway.org/)の「Exercise 4 - 6」で学んだことのまとめです。

## Exercise 4: Variables and Names

```python
cars = 100
space_in_a_car = 4
drivers = 30
passengers = 90
cars_not_driven = cars - drivers
cars_driven = drivers
carpool_capcity = cars_driven * space_in_a_car
average_passengers_par_car = passengers / cars_driven


print(f"There are {cars} cars available.")
print("There are only", drivers, "drivers available.")
print("There will be", cars_not_driven, "empty cars today.")
print("We can transport", carpool_capcity, "people today.")
print("We have", passengers,"to car pool today.")
print("We need to put about", average_passengers_par_car, "in each car.")
```

*今sublimeで開いているフォルダの中のファイルを開く:
command + t　→　ファイル名を入力
 

## Exercise 5: More Variables and Printing

```python
my_name = 'Zed A. Shaw'
my_age = 35 # not a lie
my_height = 74 # inches
my_weight = 180 # lbs
my_eyes = 'Blue'
my_teeth = 'White'
my_hair = 'Brown'
my_height_cm = my_height * 2.5

print(f"Let's talk about {my_name}.")
print(f"He's {my_height} inches tall.")
print(f"He's {my_height_cm} centimeters tall.")
print(f"He's {my_weight} pounds heavy.")
print(f"He's {my_weight / 100 * 45} kilograms heavy.")
print("Actually that's not too heavy.")
print(f"He's got {my_eyes} eyes and {my_hair} hair.")
print(f"His teeth are usually {my_teeth} depending on coffee.")

# this line is tricky, try to get it exactly right
total = my_age + my_height + my_weight
print(f"If I add {my_age}, {my_height}, and {my_weight} I get {total}.")
```

*数字(number)を文字列(string)として表示する

```python
str(my_age)
```

## Exercise 6: String and Text

```python
types_of_people = 10
x = f"There are {types_of_people} types of people."

binary = "binary"
do_not = "don't"
y = f"Those who know {binary} those who {do_not}."

# There are 10 types of people.
print(x)

# Those who know binary those who don't.
print(y)

# I said: There are 10 types of people.
print(f"I said: {x}")

# I also said: 'Those who know binary those who don't.'
print(f"I also said: '{y}'")

hilarious = False
joke_evaluation = "Isn't that joke so funny?! {}"

# Isn't that joke so funny?! False
print(joke_evaluation.format(hilarious))

w = "This is the left side of..."
e = "a string with a right side."

# This is the left side of...a string with a right side.
```  