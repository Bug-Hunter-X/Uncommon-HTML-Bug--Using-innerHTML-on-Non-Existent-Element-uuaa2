# Uncommon HTML Bug: innerHTML on Non-Existent Element

This repository demonstrates a subtle bug that can occur in HTML when attempting to modify the `innerHTML` property of an element that does not exist in the DOM.  This can lead to unexpected behavior and silent errors.  The solution involves robust error handling and checking the existence of the element before attempting modification.

## Bug

The `bug.html` file contains an example of this error. Note that the code will run without throwing errors, but it will have an unexpected outcome. The element with id 'nonExistentElement' does not exist.  This results in a silent failure without any warning. 

## Solution

The `bugSolution.html` file demonstrates how to resolve this issue by first checking for the existence of the element using `document.getElementById()` before attempting to modify its `innerHTML`.  This approach prevents errors and ensures that the code runs as expected.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your web browser.  Observe the output.
3. Open `bugSolution.html` and observe the corrected output. 
