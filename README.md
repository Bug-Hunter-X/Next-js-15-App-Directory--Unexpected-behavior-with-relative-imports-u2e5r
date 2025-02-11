# Next.js 15 App Directory: Unexpected behavior with relative imports

This repository demonstrates a bug encountered in Next.js 15's App directory when using relative imports within components.  The issue arises when importing a component from a relative path, leading to unexpected rendering behavior or runtime errors.  This is especially true when navigating between routes within the app.

## Bug Reproduction

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Observe the unexpected behavior (explained in detail below).

## Bug Solution
The solution is provided in the `bugSolution.js` file. It demonstrates how to correctly resolve the issue by ensuring the relative paths used in imports are correctly mapped within the app directory structure.  Specifically, it is crucial to understand the routing behavior of the App Router to ensure imports are resolved from the correct base path.