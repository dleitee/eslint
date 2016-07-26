# Disallow tabs in file (no-tabs)

Some people prefer whitespaces instead of tab characters in a file. So they would want to disallow tab anywhere inside a file including comments.

## Rule Details

This rule looks for tabs inside the file. It can abe anywhere inside code or comments or anything.

Examples of **incorrect** code for this rule:

```js
var a /t= 2;

/**
* /t/t its a test function
*/
function test(){}

var x = 1; // /t test
```

Examples of **correct** code for this rule:

```js
var a = 2;

/**
* its a test function
*/
function test(){}

var x = 1; // test
```

## When Not To Use It

If you have established a standard where having tabs is fine.
