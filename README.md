# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates a subtle bug related to the usage of `innerHTML` in HTML.  The bug arises from attempting to directly insert an HTML element into `innerHTML` without converting it to a string first. This leads to a JavaScript syntax error and prevents the intended content update.

## Bug Description
The bug is in the JavaScript code that manipulates the `innerHTML` property of a div element. The attempt to directly insert a `<p>` element into `innerHTML` without converting it to a string will throw a syntax error, preventing the expected text replacement.

## Solution
The solution involves converting the HTML element to a string before inserting it into `innerHTML`.  This is accomplished using the `outerHTML` property or by creating the string representation of the element manually.