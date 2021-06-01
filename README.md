# electron-app

electron bootstrap documentation to getting started

`yarn init -y`

entry point should be main.js.  

author and description can be any value, but are necessary for app packaging.  

```json
{
  "name": "my-electron-app",
  "version": "1.0.0",
  "description": "Hello World!",
  "main": "main.js",
  "author": "Jane Doe",
  "license": "MIT"
}
```
`yarn add -D electron`

```json
{
  "scripts": {
    "start": "electron ."
  }
}
```

create an index.html in path root  
```html5
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <!-- https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP -->
    <meta http-equiv="Content-Security-Policy" content="default-src 'self'; script-src 'self'">
    <meta http-equiv="X-Content-Security-Policy" content="default-src 'self'; script-src 'self'">
    <title>Hello World!</title>
  </head>
  <body>
    <h1>Hello World!</h1>
    We are using Node.js <span id="node-version"></span>,
    Chromium <span id="chrome-version"></span>,
    and Electron <span id="electron-version"></span>.
  </body>
</html>
```

create main.js  
```javascript
const { app, BrowserWindows } require("electron");

function create Window () {
  const win = new BrowserWindow({
    width: 800,
    height: 800,
  })
}
```
