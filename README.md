# Tailwind CSS @apply Directive Error: Class Not Found

This repository demonstrates a common, yet subtle, error when using Tailwind CSS's `@apply` directive.  The issue arises when referencing a class that either doesn't exist within your Tailwind configuration or contains a typo.

The problem is that this error doesn't throw a JavaScript error or warning in the console.  Instead, the affected element simply remains unstyled, making it difficult to debug.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the text is not styled as expected. The `text-wrong-color` class is not defined.

## Solution

Review your Tailwind configuration (`tailwind.config.js`) to ensure all classes used with `@apply` are correctly defined. Also, carefully double-check for typos in your class names.