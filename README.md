# Simple Parcel Boilerplate

## Install simple-parcel-boilerplate
npm install 

## To run in development mode
npm run dev

## To run in production mode
npm run build

# How to create a simple ParcelJS project

### Step 1 - Setup project

Create a new directory

```
mkdir parcel-project
```

```
cd parcel-project
```

```
npm init --yes
```

## Step 2 - Create starter file

create index.html

```
<!DOCTYPE html>
<html>
  <head>
    <title>Simple Parcel Boilerplate</title>
  </head>

  <body>
    <script src="index.js"></script>
  </body>
</html>
```

create index.js

This can be left empty

## Step 2 - Add dependencies

```
npm install parcel-bundler --save-dev
```

## Step 3 - Add scripts to package.json

change main: to "main": "index.html",

delete

```
"test": "echo \"Error: no test specified\" && exit 1"
```

and replace with

```
"dev": "parcel index.html --open",
"build": "parcel build index.html"
```

## Step 4 - Check it is working

Add a div and text to the HTML

```
var newDiv = document.createElement("div")
// and give it some content
var newContent = document.createTextNode("Hello")
// add the text node to the newly created div
newDiv.appendChild(newContent)
// add the newly created element and its content into the DOM
var currentDiv = document.getElementById("div1")
document.body.insertBefore(newDiv, currentDiv)
```

You should now be displated with the text 'Hello' 

