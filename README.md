# Lecture-5

```

      Overview
          |
  -----------------
  |       |       |
String  Methods Numbers

```

# What is a Method in JavaScript?

A method is a block of code which only runs when it is called. You can pass data, known as
parameters, into a method. Methods are used to perform certain actions, and they are also
known as functions.

```
1)CharAt(),at()       2)toString()       3)concat()      4)trim()
  5)includes()    6)IndexOf(),lastindexOf()    7)replace(),replaceAll()
                  8)substring(),slice()   9)split()
                    10)toLowerCase(),toUpperCase();

```
## 1)charAt()

The charAt() method returns the character at a
specified index (position) in a string. The index of the
first character is 0, the second 1, ... The index of the last
character is string length - 1 

### Example:
```
let str = "Hello, World!";
console.log(str.charAt(0)); // "H"
console.log(str.charAt(7)); // "W"
console.log(str.charAt(50)); // "" (empty string, out of range)

```
## 2)at()
The at() method takes an integer value and returns a
new String. This method allows for positive and
negative integers. Negative integers count back from
the last string character.

### Example:
```
let str = "Hello, World!";
console.log(str.at(0));  // "H"
console.log(str.at(-1)); // "!"
console.log(str.at(50)); // undefined (out of range)

```

## toString()

The toString() method returns a string representing
the object. By default toString() takes no
parameters

### Example:
```
let arr = [1, 2, 3, 4];
console.log(arr.toString()); // "1,2,3,4"

```
## 4)concat()
The concat() method joins two or more strings. The
concat() method returns a new string. The concat()
method does not change the original string.

### Example:
```
let str1 = "Hello";
let str2 = "World";
let result = str1.concat(", ", str2, "!");
console.log(result); // "Hello, World!"

```

## 5)trim()
The trim() method removes whitespaces from both
side of sentences. The trim() method does not
change the original string
```
let str = "   Hello, World!   ";
console.log(str.trim());  // "Hello, World!"

```

## 6)includes()
The includes() method returns true if a string contains
a specified string. Otherwise it returns false. The
includes() method is case sensitive

### Example:

```
let text = "Hello, world!";
console.log(text.includes("Hello")); // true
console.log(text.includes("hello")); // false (case-sensitive)
console.log(text.includes("world", 8)); // true (starts searching at index 8)
console.log(text.includes("World")); // false (case-sensitive)

```
## 7)indexOf()
The indexOf() method returns the position of the
first occurrence of avalue in a string. The indexOf()
method returns -1 if the value is not found. The
indexOf() method is case sensitive.


### Example:
```
let text = "Hello, world!";
console.log(text.indexOf("world"));  // 7
console.log(text.indexOf("o"));      // 4 (first 'o' found at index 4)
console.log(text.indexOf("o", 5));   // 8 (search starts from index 5)
console.log(text.indexOf("Java"));   // -1 (not found)

```

## 8)replace()
The replace() method returns a new string with the
value(s) replaced. The replace() method searches a
string for a value or a regular expression. The replace()
method does not change the original string.

### Example:
```
let text = "Hello, world!";
let newText = text.replace("world", "JavaScript");
console.log(newText); // "Hello, JavaScript!"

```

## 9) substring()

Black Arrow Paint Stroke Scribble
Handdrawn Curved Arrow
 The substring(start,end) method extracts characters,
between two indices (positions), from a string, and
returns the substring. The substring() method extracts
characters from start to end (exclusive). The substring()
method does not change the original string. If start is
greater than end, arguments are swapped: (4, 1) = (1, 4).
Start or end values less than 0, are treated as 0.

### Example:
```
let text = "JavaScript";
console.log(text.substring(0, 4));  // "Java"
console.log(text.substring(4));     // "Script" (from index 4 to the end)
```


## 10)slice()
The slice(start,end) method returns a shallow copy of a
portion of an array and string into a new array object
selected from start to end ( end not included) where
start and end represent the index of items in that array.

### Example:
```
let text = "JavaScript";
console.log(text.slice(0, 4));  // "Java"
console.log(text.slice(4));     // "Script" (from index 4 to the end)
```
## 11)toLowerCase()
The toLowerCase() method converts a string to
lowercase letters. The toLowerCase() method does not
change the original string.

### Example:
```
let text = "HeLLo WoRLd";
console.log(text.toLowerCase()); // "hello world"
```

## 12)toUpperCase()
The toUpperCase() method converts a string to
lowercase letters,using this locale The toUpperCase()
method does not change the original string.

### Example:

```
let text = "JavaScript";
console.log(text.toUpperCase()); // "JAVASCRIPT"
```
## 13)Split()

The split() method splits a string into an array of substrings. The split() method
returns the new array. The split() method does not change the original string. If (" ") is
used as separator, the string is split between words.

### Example:
```
let text = "apple,banana,cherry";
let fruits = text.split(",");
console.log(fruits); // ["apple", "banana", "cherry"]
```
