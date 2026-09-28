# Copilot Skills Demo

This repository is a small demo workspace for exploring GitHub Copilot in VS Code and GitHub Codespaces. Its JavaScript files are short examples that can be read, edited, or extended with Copilot.

## What's Included

- `comments.js` creates an Express web server on port 3000. A request to `/` receives the text `Hello, World!`, and the server logs its local URL when it starts. The example calls `express()` but does not import Express; to run it as a CommonJS script, install Express with `npm install express` and add `const express = require('express');` at the top.
- `member.js` and `skills.js` each define `calculateNumbers(var1, var2)`. The function returns an object containing the sum, difference, product, and quotient of its inputs. If the second input is zero, the quotient is the string `'undefined'` instead of dividing by zero. These two files currently contain the same implementation.
- `.devcontainer/devcontainer.json` configures a Codespace using the base Ubuntu development container image and recommends the GitHub Copilot VS Code extension.

## Running the Web Server

After installing Express and adding the import described above, run:

```sh
node comments.js
```

Then open [http://localhost:3000](http://localhost:3000) to see the response.