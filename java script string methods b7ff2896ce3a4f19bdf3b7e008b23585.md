# java script string methods

## Note

String **search** methods are covered in the next chapter.

## JavaScript String Length

The `length` property returns the length of a string:

### Example

let text = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

let length = text.length;

[Try it Yourself »](https://www.w3schools.com/js/tryit.asp?filename=tryjs_string_length)

## Extracting String Parts

There are 3 methods for extracting a part of a string:

- `slice(*start*, *end*)`
- `substring(*start*, *end*)`
- `substr(*start*, *length*)`

## JavaScript String slice()

`slice()` extracts a part of a string and returns the extracted part in a new string.

The method takes 2 parameters: start position, and end position (end not included).

## JavaScript String substring()

`substring()` is similar to `slice()`.

The difference is that start and end values less than 0 are treated as 0 in `substring()`.

If you omit the second parameter, `substring()` will slice out the rest of the string.

## JavaScript String substr()

`substr()` is similar to `slice()`.

The difference is that the second parameter specifies the **length** of the extracted part.

If you omit the second parameter, `substr()` will slice out the rest of the string.

If the first parameter is negative, the position counts from the end of the string.

## Replacing String Content

The `replace()` method replaces a specified value with another value in a string:

By default, the `replace()` method replaces **only the first** match:

By default, the `replace()` method is case sensitive. Writing MICROSOFT (with upper-case) will not work:

To replace case insensitive, use a **regular expression** with an `/i` flag (insensitive):

To replace all matches, use a **regular expression** with a `/g` flag (global match):

## JavaScript String ReplaceAll()

In 2021, JavaScript introduced the string method `replaceAll()`:

The `replaceAll()` method allows you to specify a regular expression instead of a string to be replaced.

If the parameter is a regular expression, the global flag (g) must be set, otherwise a TypeError is thrown.

## Converting to Upper and Lower Case

A string is converted to upper case with `toUpperCase()`:

A string is converted to lower case with `toLowerCase()`:

## JavaScript String toUpperCase()

## JavaScript String toLowerCase()

## JavaScript String concat()

`concat()` joins two or more strings:

The `concat()` method can be used instead of the plus operator. These two lines do the same:

## JavaScript String trim()

The `trim()` method removes whitespace from both sides of a string:

## JavaScript String trimStart()

[ECMAScript 2019](https://www.w3schools.com/js/js_2019.asp) added the String method `trimStart()` to JavaScript.

The `trimStart()` method works like `trim()`, but removes whitespace only from the start of a string.

JavaScript String `trimStart()` is supported in all modern browsers since January 2020:

## JavaScript String trimEnd()

[ECMAScript 2019](https://www.w3schools.com/js/js_2019.asp) added the string method `trimEnd()` to JavaScript.

The `trimEnd()` method works like `trim()`, but removes whitespace only from the end of a string.

JavaScript String `trimEnd()` is supported in all modern browsers since January 2020:

## JavaScript String Padding

[ECMAScript 2017](https://www.w3schools.com/js/js_2017.asp) added two new string methods to JavaScript: `padStart()` and `padEnd()` to support padding at the beginning and at the end of a string.

## JavaScript String padStart()

The `padStart()` method pads a string from the start.

It pads a string with another string (multiple times) until it reaches a given length.

## Browser Support

`padStart()` is an [ECMAScript 2017](https://www.w3schools.com/js/js_2017.asp) feature.

It is supported in all modern browsers:

`padStart()` is not supported in Internet Explorer.

## JavaScript String padEnd()

The `padEnd()` method pads a string from the end.

It pads a string with another string (multiple times) until it reaches a given length.

## Browser Support

`padEnd()` is an [ECMAScript 2017](https://www.w3schools.com/js/js_2017.asp) feature.

It is supported in all modern browsers:

`padEnd()` is not supported in Internet Explorer.

## Extracting String Characters

There are 3 methods for extracting string characters:

- `charAt(*position*)`
- `charCodeAt(*position*)`
- Property access [ ]

## JavaScript String charAt()

The `charAt()` method returns the character at a specified index (position) in a string:

## JavaScript String charCodeAt()

The `charCodeAt()` method returns the unicode of the character at a specified index in a string:

The method returns a UTF-16 code (an integer between 0 and 65535).

## Property Access

ECMAScript 5 (2009) allows property access [ ] on strings:

## Converting a String to an Array

## JavaScript String split()

A string can be converted to an array with the `split()` method:

If the separator is omitted, the returned array will contain the whole string in index [0].

If the separator is "", the returned array will be an array of single characters: