# CSS Centering Issue with Percentage-Based Dimensions

This repository demonstrates an uncommon issue related to centering elements in CSS when using percentage-based widths and heights.  The problem arises from the interaction of `margin: auto;` with percentage values. While `margin: auto;` typically centers block-level elements horizontally, it doesn't reliably center vertically when percentages are involved.

The `bug.css` file contains the problematic CSS, and `bugSolution.css` shows a solution.

## Problem

The goal is to center a blue square (`.container`) within a red square (`div`).  The use of percentages for width and height simplifies responsiveness, but causes the unexpected centering behavior.

## Solution

The solution involves using `display: flex` on the parent container (`div`) and setting `align-items: center;` and `justify-content: center;` to correctly center the child element both horizontally and vertically.