# pluralsight-js-core-language
Pluralsight Path - JavaScript Core Language

## JavaScript: Getting Started

JavaScript Applications
- Web Pages
- Business Apps
- Utility Apps
- Games

Content
- JavaScript programming
- Those who are new to JavaScript
- JavaScript features
- Build a card game Blackjack

### Introduction to JavaScript

#### Intoduction

- TypeScript - superset of JavaScript that compiles to plain JavaScript
- Apache Cordova - Native apps for smartphones and tablets
- Electron - Mac and Windows Desktop apps
- NodeJS - Server-side code

#### Installing Development Software

```bash
git --version
```

If you don't have it you can download it here:
https://git-scm.com/downloads

```bash
npm --version
```

If you don't have it you can download it here:
https://nodejs.org/en/

Code Editor - https://code.visualstudio.com/

#### Hello World Project from GitHub

https://github.com/pluralsight/web-dev-starter
Code > Clone with HTTPS 

```bash
git clone https://github.com/pluralsight/web-dev-starter.git
```

```bash
npm install
```

```bash
npm start
```

It'll open http://localhost:3000/ with our Hello World example


### JavaScript Beginnings

#### Introduction
- Adding JavaScript Code to HTML
- Multiple JavaScript Files
- Formatting Code
- Detecting and Fixing Errors
- Case Sensitivity
- Commenting Code

#### Adding JavaScript Coode to a Web Page

JavaScript in index.html
```JS
<script>

    //JavaScript code goes here ...
    
</script>
```

Example
```JS
<script>
    alert('Hello world!');
    alert('Carved Rock Fitness');
</script>
```

#### Working with JavaScript Files

JavaScript in index.html

```JS
<script src="./filename.js"></script>
```

```JS
<script src="./utils.js"></script>
<script src="./home.js"></script>
```

Create home.js in the same folder of index.html

**home.js**
```JS
alert('Hello world!');
alert('Second Message');
```

Create utils.js in the same folder of index.html

**utils.js**
```JS
function showMessage(message) {
    document.getElementById('message').textContent = message;
}
```

On index.html add that id
```html
<h1 id="message" class="col-sm-12">GET A GRIP</h1>
```

**home.js**
```JS
// show the title
showMessage("Title...");
let price = 149.99;
/*
    Detail complex logic...
    Some algorithm...

*/
```
