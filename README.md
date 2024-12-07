# Uncommon HTML Bug: DOM Manipulation Timing Issue

This repository demonstrates an uncommon bug in HTML related to the timing of DOM manipulation. The script attempts to modify the content of a div element before the DOM is fully loaded, resulting in no visible changes. The solution involves using the DOMContentLoaded event to ensure that the script executes after the DOM is ready.

## Bug Description

The `bug.html` file contains a simple HTML page with a div element and a script that attempts to modify the div's content. The script runs before the browser has fully parsed and built the DOM tree. Thus the modification does not take effect. 

## Solution

The `bugSolution.html` file demonstrates the solution. It uses the `DOMContentLoaded` event to ensure that the script is only executed after the DOM is ready.