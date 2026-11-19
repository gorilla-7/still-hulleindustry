# Running and publishing

This imported project is a static HTML page. It redirects visitors to
`https://www.google.com`, preserving the URL fragment (the part after `#`).

No dependencies or secrets are required.

## Preview

Use the **Preview site** workflow. It copies `index.html` into `dist/` and serves
that directory on port 5000 with Python's development HTTP server.
The browser immediately navigates away to Google; an embedded preview may block
that external navigation.

## Publish

Publishing uses a Static deployment. Its build command copies only `index.html`
into `dist/`, and `dist/` is the public directory. No production server is needed.
Click **Publish** in Replit to make the site live.

`dist/` is generated and excluded from source control and upload; publishing
recreates it from `index.html`.
