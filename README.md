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

#### Formatting Code

- Only add blank lines and tabs if it helps to read your code easily

#### Detecting and Fixing Errors

Inspect > Console
**home.js**
```JS
showMessage("Title...");

console.log("any message...");
```

#### Case Sensitivity

**home.js**
```JS
ShowMessage("Title...");
```

This will throw an error "Uncaught ReferenceError: ShowMessage is not defined"

**home.js**
```JS
showmessage("Title...");
```

This will throw an error "Uncaught ReferenceError: showmessage is not defined"

#### Commenting Code

Comments

```JS
// Single line comment

/*
    Multiple line comment
    Add as many lines as you like
*/
```

#### Summary

**Including JS in HTML**
- <script> </script>
- <script src="./filename.js"></script>

**Formatting Code**
- Freely use whitespace

**Detecting Errors**

**Case Sensitivity**
- JS is case sensitive

**Commenting Code**
- // single line comment
- /* multiple line comment */

### Variables and Constants

#### Introduction
- Whats is a Variable?
- Declaring Variables
- Naming Variables
- Common Error Using Variables
- Changing Variable Values
- Constants
- The var Keyword

#### What Is a Variable?

#### Declaring Variables

```JS
let total = 149.99;

let product = 'Hiking Boots';

let discounted = true;
```

#### Using let to Declare Variables

**home.js**
```JS
let welcome = 'Welcome';

let price = 49.99;
let name = 'Hiking Boots';
let discounted = false;

let price = 49.99,
    name = 'Hiking Boots',
    discounted = false;

showMessage(welcome);
```

#### Naming Variables

**Valid Variable Names**
- Start with One of: **_ $ letter**
- Followed by Zero or More: **_ $ letter number**

```JS
a
account
account_99
accountNumber
_accountNumber
$accountNumber
_123
__proto__
```

#### Common Errors Using Variables

**home.js**
```JS
let 99times = 99;
showMessage(99times);
```

This will throw the error "Uncaught SyntaxtError: Invalid or unexpected token"

**home.js**
```JS
let times99 = 99;
let _times99 = 99;
showMessage(times99);
```

Variable names cannot have spaces and cannot be keywords

**home.js**
```JS
let let = 99;
showMessage(let);
```

This will throw the error "Uncaught SyntaxtError: let is disallowed as a lexically bound name"

**home.js**
```JS
let price;
showMessage(price);
```

This will throw the message "undefined"

#### Changing Variable Values

**home.js**
```JS
let price = 99.99;

// lots of code ...

price = 49.99;

// more code here ...

price = 29.99;

showMessage(price);
```

#### Constants

**home.js**
```JS
const price = 40;

// lots of code ...

price = 49.99;

showMessage(price);
```

This will throw the error "Uncaught TypeError: Assigment to constant variable"

**home.js**
```JS
const price;

showMessage(price);
```

This will throw the error "Uncaught SyntaxError: Missing initializer in const declaration"

#### The var Keyword

**home.js**
```JS
var price = 25;

showMessage(price);
```

**home.js**
```JS
showMessage(price);

let price = 25;
```

This will throw the error "Uncaught ReferenceError: Cannot access 'price' before initialization"

**home.js**
```JS
showMessage(price);

var price = 25;
```

This won't show any error

**home.js**
```JS
showMessage(price);
console.log(price);

var price = 25;
```

This will throw the message "undefined"

#### Summary

**Defined Variables**

**Declared Variables Using let**

**Naming Variables**
- Begin with: _ $ letter
- Then 0 or more: _ $ letter number

**Common Errors Using Variables**

**Variables Change Over Time**

**Declaring Constants**
- The const Keyword

**The var Keyword**
- Avoid it, use let or const instead



