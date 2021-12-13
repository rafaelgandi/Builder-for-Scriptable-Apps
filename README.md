# 🤖 Builder for Scriptable Apps
Simple node js script to concatenate files for building a Scriptable mini app.

# Installation
Just copy the `builder.js` file to where you want to build your scriptable mini app.

## Create a new app
```
node builder create <name of app>
```
This will create a template file/directory structure for your app. File structure would look like this:
```
|- builder.js
|- src/
|--- src.html
```

## Watching for changes on file save
```
node builder watch
```
This will concatenate any changes to your files inside the `src` to the `index.html`(created on save) when file is saved. File structure will now look like this: 
```
|- builder.js
|- index.html
|- src/
|--- src.html
|--- styles.css
|--- index.js
|--- other.js
```

## ⚠️ Note
- File named `index.js` inside the `src` directory will always be prepended on concatination of js codes.
- For updating any html markup, just update `src.html` file.

