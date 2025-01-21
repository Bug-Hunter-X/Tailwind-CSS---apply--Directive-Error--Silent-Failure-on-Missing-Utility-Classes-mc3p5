# Tailwind CSS `@apply` Directive Error: Silent Failure on Missing Utility Classes

This repository demonstrates an uncommon error in Tailwind CSS related to the `@apply` directive.  When using `@apply` with a nonexistent or misspelled utility class, Tailwind doesn't always throw a clear error. Instead, the class simply doesn't get applied, leading to unexpected visual results.  This can be difficult to debug.

The `bug.html` file showcases the problematic code. The `bugSolution.html` file demonstrates how to solve it.

## How to reproduce

1. Clone this repository.
2. Make sure you have Node.js and npm installed.
3. Install Tailwind CSS: `npm install -D tailwindcss postcss autoprefixer`
4. Initialize Tailwind: `npx tailwindcss init`
5. Run the development server (details in `package.json`) and observe the behavior.

## Solution

Carefully review your `tailwind.config.js` file and ensure all the utility classes used within `@apply` directives are correctly defined. Double check for typos.