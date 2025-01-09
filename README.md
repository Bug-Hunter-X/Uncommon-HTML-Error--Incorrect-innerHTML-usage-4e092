# Uncommon HTML Error: Incorrect innerHTML usage

This repository demonstrates an uncommon error related to the use of `innerHTML` in HTML. The error occurs when a non-string value is assigned to the `innerHTML` property of an element, leading to unexpected behavior. While `innerHTML` generally expects string values, assigning a number or another data type can cause issues. This example showcases this issue and provides a solution.

## Bug Description
The bug arises from attempting to set the `innerHTML` property of a div element to a number instead of a string. This results in unexpected behavior as the browser attempts to interpret the numerical value as HTML content which isn't correct. In this case, nothing is rendered at all.  This is different from the common error of incorrectly escaping HTML entities.

## Solution
The solution is straightforward: Ensure that the value assigned to `innerHTML` is always a string. You can achieve this by explicitly converting non-string values to strings using the `toString()` method.