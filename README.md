# MongoDB $inc Operator Error: Using String Instead of Number

This repository demonstrates an uncommon error related to the MongoDB `$inc` operator.  The error occurs when a string value is provided for the increment instead of a numerical value. This leads to unexpected behavior, typically an error or unintended data modification.

## Problem Description

The `$inc` operator is used to increment or decrement a numeric field in a MongoDB document.  However, if you mistakenly supply a string instead of a number as the increment value, MongoDB will not perform the intended operation.

## Bug Reproduction

The `bug.js` file contains the erroneous code.  Running this code against a MongoDB instance will trigger the error.

## Solution

The correct usage of the `$inc` operator involves providing a numerical value for the increment.  The `bugSolution.js` file demonstrates the corrected code.

## How to run the example

1.  Make sure you have Node.js and a MongoDB instance running.
2.  Clone this repository.
3.  Run `npm install` to install any necessary dependencies (if any are needed).
4.  Run `node bug.js` to reproduce the error.
5.  Run `node bugSolution.js` to see the corrected code in action.