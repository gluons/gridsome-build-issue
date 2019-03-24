# Gridsome build issue

A repo to repro Gridsome build error.

## Steps to repro

1. Run in dev mode.  
   ```bash
   yarn dev
   ```

   It works perfectly.

2. Build project.  
   ```bash
   yarn build
   ```

   **Get this error:**
   ```
   (function (exports, require, module, __filename, __dirname) { label.radio-toggle-button {
                                                                                        ^

   SyntaxError: Unexpected token {
   ```
