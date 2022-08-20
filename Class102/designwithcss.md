# Cascading Style Sheets

**CSS is a rule based language - you define rules by specifying groups of styles that apply to elements to your page**

Example:
```
h1 {
    color: red;
    font-size: 5em;
}
```
the h1 in the example is a selector while color and font-size are properties.

All web standards technologies (HTML, CSS, JavaScript, etc.) are defined in giant documents called specifications (or "specs"), which are published by standards organizations (such as the W3C, WHATWG, ECMA, or Khronos) and define precisely how those technologies are supposed to behave.

## How to add CSS

There are three ways: External, Internal, and Inline

**External**:
```
<link rel="stylesheet" href="stylesheet.css">
```
**Internal**:
```
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
```
**Inline**:
```
<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>
```

**Reference guides**:

[W3schools](https://www.w3schools.com/cssref/default.asp) <br>
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)

[Back to main page](https://vadengrey.github.io/reading-notes/)

