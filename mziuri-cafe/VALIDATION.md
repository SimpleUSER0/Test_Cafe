# Validation

Passed:
- `npm run check`: server and frontend JavaScript syntax.
- Every local HTML asset exists, including three WebP images.
- Every section anchor resolves to an existing element.
- HTTP 200: page, CSS, JS, each image, `/health`.
- HTTP 404 for missing pages.

Responsive CSS targets desktop, tablet and mobile, including 780px and 420px breakpoints. Browser rendering and interactive end-to-end checks could not be run because the browser executable was unavailable and its download failed in the execution environment. Before production, inspect the page at 1440px, 768px, 390px and 320px; click all menu categories, open/close the mobile navigation and open/close gallery images with Escape.

This repository has not been pushed to GitHub or deployed to Railway. Follow README.md to connect your accounts and publish.
