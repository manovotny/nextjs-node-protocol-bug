# nextjs-node-protocol-bug

Minimal reproducable example of this issue: https://github.com/vercel/next.js/issues/28774

## Steps to reproduce

1. Clone repo.
1. Run `npm run dev`.
1. [Toggle the two `import process` lines in `pages/index.js`](https://github.com/manovotny/nextjs-node-protocol-bug/blob/main/pages/index.js#L5-L6) to see it working / not working.

## Errors

```
Module build failed: UnhandledSchemeError: Reading from "node:process" is not handled by plugins (Unhandled scheme).
Webpack supports "data:" and "file:" URIs by default.
You may need an additional plugin to handle "node:" URIs.
```
