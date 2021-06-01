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


