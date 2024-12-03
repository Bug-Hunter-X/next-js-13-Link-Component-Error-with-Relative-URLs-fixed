# Next.js 13 Link Component Issue

This repository demonstrates a common error encountered when using the Next.js `Link` component with relative URLs after upgrading to Next.js 13. The issue arises from changes in how Next.js handles routing and page resolution.

## Problem

The `Link` component, with a simple relative URL like `/about`, fails to navigate correctly. This may happen due to the absence of an `about.js` file in the `pages` directory or incorrect file structure. 

## Solution

Ensure the page you are trying to link to exists in your `pages` directory, mirroring the URL path. This involves creating the file named `pages/about.js` and then updating the link. The fix may also involve checking the base path config for your application and ensuring that all pages are correctly configured.

## Setup

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Start the development server using `npm run dev`.
4. Navigate to the page with the broken link and test the fix.