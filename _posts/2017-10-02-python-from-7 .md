---
layout: post
title:  "Learn Python 3 the Hard Way: Exercise 7 - 9で学んだこと"
---

[Learn Python 3 the Hard Way](https://learnpythonthehardway.org/)の「Exercise 7 - 9」で学んだことのまとめです。

## Exercise 7: More Printing

```python
# Mary had a little lamb.
print("Mary had a little lamb.")

# Its fleece was white as snow.
print("Its fleece was white as {}.".format('snow'))

# And everywhere that Mary went.
print("And everywhere that Mary went.")

# ..........
print("." * 10) # what'd that do?

end1 = "C"
end2 = "h"
end3 = "e"
end4 = "e"
end5 = "s"
end6 = "e"
end7 = "B"
end8 = "u"
end9 = "r"
end10 = "g"
end11 = "e"
end12 = "r"

# watch that comma at the end. try removing it to see what happens
# →
# File "ex7/ex7.py", line 29
#   print(end1 + end2 + end3 + end4 + end5 + end6 end=' ')                                               ^
# SyntaxError: invalid syntax

# Cheese Burger
# end=' 'を入れることで改行されない
print(end1 + end2 + end3 + end4 + end5 + end6, end=' ')
print(end7 + end8 + end9 + end10 + end11 + end12)
```

## Exercise 8: Printing, Printing

```python
# .format()の中の4つの文字列を1行目のformatterの形に渡して出力する
formatter = "{} {} {} {}"

print(formatter.format(1, 2, 3, 4))
print(formatter.format("one", "two", "three", "four"))

# TrueとFalseは、Pythonの中では文字列ではなくkeywordsとして認識されるので
# ""をつけない
print(formatter.format(True, False, False, True))
print(formatter.format(formatter, formatter, formatter, formatter))
print(formatter.format(
 	"Try your",
 	"Own text here",
 	"Maybe a poem",
 	"Or a song about fear"
))

# 最後の5が無視される
print(formatter.format(1, 2, 3, 4, 5))
```

## Exercise 9: Printing, Printing, Printing

```python
# Here's some new strange stuff, remember type it exactly.

days = "Mon Tue Wed Thu Fri Sat Sun"

# 改行→改行したい文字列の前に\n(\ = option + ¥)
months = "Jan\nFeb\nMar\nApr\nMay\nJun\nJul\nAug"

print("Here are the days: ", days)
print("Here are the months: ", months)

# """で文字列をはさむと全て文字列と認識される/文字列を改行できる
print("""
There's something going on here.
With the three double-quotes.
We'll be able to type as much as we like.
Even 4 lines if we want, or 5, or 6.
""")

# "が3つじゃないと、
# 'で文字列が途切れたり、文字列として認識されなかったりするのでエラーになる	

# SyntaxError: EOL while scanning string literal
print("
There's something going on here.
With the three double-quotes.
We'll be able to type as much as we like.
Even 4 lines if we want, or 5, or 6.
")
```