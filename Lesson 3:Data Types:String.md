## **What is a String?**  
📌 A **string** in Python is a **sequence of characters** enclosed in quotes (`"Hello"` or `'Python'`).  
It can contain **letters, numbers, symbols, and spaces**.  

---

## **What are Python String Methods & Why Do We Need Them?**  
📌 **Python has 47 built-in string methods** that help modify and analyze text easily.  
They allow us to **change case, remove spaces, replace words, split text, and search within strings**.  

📌 **We need them to process text efficiently** without writing complex code, making tasks like **formatting, searching, and cleaning text simpler**.  

📌 **String methods can also be combined** to create **more powerful and flexible operations**, allowing advance

| #  | Method               | What It Does                         | Example |
|----|----------------------|--------------------------------------|---------|
| 1  | `.lower()`           | Converts text to lowercase          | `"HELLO".lower()` → `"hello"` |
| 2  | `.upper()`           | Converts text to uppercase          | `"hello".upper()` → `"HELLO"` |
| 3  | `.strip()`           | Removes spaces from both sides      | `" hello ".strip()` → `"hello"` |
| 4  | `.replace(old, new)` | Replaces part of a string           | `"apple".replace("a", "o")` → `"opple"` |
| 5  | `.split(",")`        | Splits a string into a list         | `"a,b,c".split(",")` → `["a", "b", "c"]` |
| 6  | `.find("word")`      | Finds the index of a substring      | `"hello".find("o")` → `4` |
| 7  | `.startswith("word")`| Checks if string starts with something | `"Hello".startswith("H")` → `True` |
| 8  | `.endswith("word")`  | Checks if string ends with something | `"Hello".endswith("o")` → `True` |
| 9  | `.title()`           | Capitalizes the first letter of each word | `"hello world".title()` → `"Hello World"` |
| 10 | `.capitalize()`      | Capitalizes only the first letter   | `"hello".capitalize()` → `"Hello"` |
| 11 | `.count("word")`     | Counts occurrences of a substring   | `"apple apple".count("apple")` → `2` |
| 12 | `.lstrip()`          | Removes spaces from the left        | `" hello".lstrip()` → `"hello"` |
| 13 | `.rstrip()`          | Removes spaces from the right       | `"hello ".rstrip()` → `"hello"` |
| 14 | `.join(list)`        | Joins a list into a string          | `",".join(["a", "b"])` → `"a,b"` |
| 15 | `.zfill(n)`          | Adds leading zeros                  | `"5".zfill(3)` → `"005"` |
| 16 | `.isalpha()`         | Checks if only letters              | `"hello".isalpha()` → `True` |
| 17 | `.isdigit()`         | Checks if only numbers              | `"123".isdigit()` → `True` |
| 18 | `.isalnum()`         | Checks if only letters & numbers    | `"hello123".isalnum()` → `True` |
| 19 | `.isspace()`         | Checks if string is only spaces     | `"   ".isspace()` → `True` |
| 20 | `.isnumeric()`       | Checks if string is a number        | `"1234".isnumeric()` → `True` |
| 21 | `.swapcase()`        | Swaps uppercase & lowercase         | `"HeLLo".swapcase()` → `"hEllO"` |
| 22 | `.rfind("word")`     | Finds last occurrence of a word     | `"apple apple".rfind("apple")` → `6` |
| 23 | `.index("word")`     | Like `.find()`, but raises error if not found | `"hello".index("o")` → `4` |
| 24 | `.rindex("word")`    | Like `.rfind()`, but raises error if not found | `"hello hello".rindex("o")` → `10` |
| 25 | `.rjust(n)`          | Right-aligns text with spaces       | `"hi".rjust(5)` → `"   hi"` |
| 26 | `.ljust(n)`          | Left-aligns text with spaces        | `"hi".ljust(5)` → `"hi   "` |
| 27 | `.center(n)`         | Centers text with spaces            | `"hi".center(6)` → `"  hi  "` |
| 28 | `.casefold()`        | Like `.lower()`, but stronger for different alphabets | `"HELLO".casefold()` → `"hello"` |
| 29 | `.format()`          | Formats text dynamically            | `"Hello {}".format("World")` → `"Hello World"` |
| 30 | `.format_map()`      | Similar to `.format()`, but uses a dictionary | `"Name: {name}".format_map({"name": "Alice"})` → `"Name: Alice"` |
| 31 | `.partition("sep")`  | Splits into 3 parts: before, separator, after | `"hello:world".partition(":")` → `("hello", ":", "world")` |
| 32 | `.rpartition("sep")` | Like `.partition()`, but from the right | `"a:b:c".rpartition(":")` → `("a:b", ":", "c")` |
| 33 | `.encode()`          | Converts a string into bytes        | `"hello".encode()` → `b'hello'` |
| 34 | `.expandtabs(n)`     | Sets tab size                       | `"a\tb".expandtabs(4)` → `"a   b"` |
| 35 | `.isdecimal()`       | Checks if a string is a decimal number | `"123".isdecimal()"` → `True` |
| 36 | `.isascii()`         | Checks if all characters are ASCII  | `"Hello!".isascii()` → `True` |
| 37 | `.isidentifier()`    | Checks if string is a valid variable name | `"hello_1".isidentifier()` → `True` |
| 38 | `.translate(table)`  | Replaces characters using a table   | `"hello".translate({104: "H"})` → `"Hello"` |
| 39 | `.maketrans()`       | Creates a translation table         | `"hello".maketrans("h", "H")` |
| 40 | `.removeprefix("word")` | Removes prefix from a string     | `"HelloWorld".removeprefix("Hello")` → `"World"` |
| 41 | `.removesuffix("word")` | Removes suffix from a string     | `"filename.txt".removesuffix(".txt")` → `"filename"` |
| 42 | `.splitlines()`      | Splits string by lines              | `"hello\nworld".splitlines()` → `["hello", "world"]` |
| 43 | `.capatilize()`      | Capitalizes the first letter        | `"hello".capitalize()"` → `"Hello"` |
| 44 | `.rstrip("chars")`   | Removes specified characters from the right | `"hello!!!".rstrip("!")` → `"hello"` |
| 45 | `.lstrip("chars")`   | Removes specified characters from the left | `"!!!hello".lstrip("!")` → `"hello"` |
| 46 | `.upper().lower().capitalize().title()` | Changes case of string | `"hello".upper()"` → `"HELLO"` |
| 47 | `.swapcase()`        | Swaps uppercase & lowercase         | `"Python".swapcase()"` → `"pYTHON"` |
| 48 | `.isprintable()`     | Checks if all characters are printable | `"\n".isprintable()` → `False` |
| 49 | `.isascii()`         | Checks if all characters are ASCII  | `"Hello!".isascii()"` → `True` |
| 50 | `.isidentifier()`    | Checks if string is a valid Python variable name | `"var1".isidentifier()` → `True` |
| 51 | `.translate(table)`  | Maps characters based on a table    | `"hello".translate(str.maketrans("h", "H"))` → `"Hello"` |
| 52 | `.expandtabs(n)`     | Expands tab characters into spaces  | `"a\tb".expandtabs(4)` → `"a   b"` |








