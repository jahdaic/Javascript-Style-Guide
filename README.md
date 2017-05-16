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
