# Javascript Style Guide

> “Arguments over style are pointless. There should be a style guide, and you should follow it”
> -Rebecca Murphey

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

### Tabs For Indentation

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

### Braces On Their Own Line

Your opening braces go on the same line as the statement.

```js
// Right
if (true)
{
	console.log('winning');
}

// Wrong
if (true) {
	console.log('losing');
}
```

### Declare One Variable Per Var Statement

Declare one variable per var statement, it makes it easier to re-order the lines. However, ignore Crockford when it comes to declaring variables deeper inside a function, just put the declarations wherever they make sense.

```js
// Right
var keys   = ['foo', 'bar'];
var values = [23, 42];
var object = {};
var key;

// Wrong
var keys = ['foo', 'bar'],
    values = [23, 42],
    object = {},
    key;
```

## Naming Conventions

### Lower Camel Case For Variables, Properties And Function Names

Variables, properties and function names should use lowerCamelCase. They should also be descriptive. Single character variables and uncommon abbreviations should generally be avoided.

```js
// Right
var adminUser = db.query('SELECT * FROM users ...');

// Wrong
var admin_user = db.query('SELECT * FROM users ...');
```

### Upper Camel Case For Class Names

Class names should be capitalized using UpperCamelCase.

```js
// Right
function BankAccount() {}

// Wrong
function bank_Account() {}
```

### Use Uppercase For Constants

Constants should be declared as regular variables or static class properties, using all uppercase letters.

```js
// Right
var SECOND = 1 * 1000;

function File() {}
File.FULL_PERMISSIONS = 0777;

// Wrong
const SECOND = 1 * 1000;

function File() {}
File.fullPermissions = 0777;
```
