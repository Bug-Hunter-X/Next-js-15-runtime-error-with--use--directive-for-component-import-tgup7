# Next.js 15 runtime error with `use` directive for component import

This repository demonstrates a runtime error encountered in a Next.js 15 application when utilizing the `use` directive to import a component. The error arises during server-side rendering (SSR) and results in a failure to render the application correctly.

## Bug Description
The issue occurs when importing a component using the `use` directive within a page component.  The error is thrown during SSR, preventing the app from rendering properly. This is not reproducible in all scenarios and is suspected to be related to interactions with specific components or libraries.

## Steps to Reproduce
1. Clone this repository.
2. Install dependencies using `npm install`.
3. Run the development server using `npm run dev`.
4. Observe the runtime error in the browser's console.

## Solution
The solution involves changing the way components are imported to avoid triggering the bug. In this case, switching from the `use` directive to a standard `import` statement resolves the error.

## Additional Notes
The exact cause of the bug is yet to be determined. It might be related to a specific interaction between the `use` directive, the imported component, and the SSR process in Next.js 15. Further investigation may be necessary to identify the root cause.