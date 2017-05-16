# Javascript Style Guide

## Basic Rules

* Tabs for indentation
* Spaces for spacing (ex. lining up variable declarations)
* Single quotes for strings, except to avoid escaping
* No unused variables
* Always use semicolons
* Space after keywords if (condition) { ... }
* Space after function name function name (arg) { ... }
* Always use === instead of == when possible, but obj == null is allowed to check null or undefined.
* Always prefix browser globals with window – except document and navigator are okay

## Formatting

### Tabs for Indentation

Use tabs for indenting your code. Displaying tabs as 4 spaces is recommended in your editor, but that's really up to personal choice. Spaces are used for spacing/lining up content.

```js
function test()
{
	var foo    = 1;
	var manchu = 3;
}
```

### Newlines

Use UNIX-style newlines (\n), and a newline character as the last character of a file. Windows-style newlines (\r\n) are forbidden inside any repository.

### No Trailing Whitespace

Just like you brush your teeth after every meal, you clean up any trailing whitespace in your JS files before committing. Otherwise the rotten smell of careless neglect will eventually drive away contributors and/or co-workers.

### Use Semicolons

According to scientific research, the usage of semicolons is a core value of our community. Consider the points of the opposition, but be a traditionalist when it comes to abusing error correction mechanisms for cheap syntactic pleasures.

### Line Length

Generally limit your lines to 100 characters. Don't feel too bad for going over, though. Sometimes going a little bit longer makes code easier to read than breaking it up into multiple lines.

### Use Single Quotes

Use single quotes, unless you are writing JSON or to avoid escaping.

```js
// Right
var foo = 'bar';

// Wrong
var foo = "bar";
```
