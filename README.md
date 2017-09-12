# Webdev 2 Javascript
### Webdev II: ATTACK OF THE JAVASCRIPT

## Intro/Goals

Today we're going to be learning how to integrate javascript in a basic webpage!! Nice! **Make sure you bring a laptop!**

Basically, javascript is going to let our web page actually *do* things, as opposed to just look pretty. Note: Javascript is totally different and unrelated to Java. idk why they named them that way, it's dumb.

### What we need

We're going to be working with HTML and CSS, and saving our projects on Github. You can see my tutorial on setting up Github and a basic HTML/CSS webpage [here](https://github.com/hacksu/Github-and-Webdev-Basics). 

Alternately, you can just use the HTML and CSS file in this repo.

## Setting up our JS file

If you haven't already, figure out what github repo you want to work in. You can set up a new one via github and clone it to your desktop, or you can work in the one we set up last time. Remember, the commands to navigate to a folder in your terminal or in Powershell are `ls` to list the contents of your current folder and `cd myFolder` to go inside another folder.

Inside the folder you want to work in, create a new file, and call it something like `script.js`. In that script, type:

`alert('hello world!');`

Now save the script, and go into your HTML file. In the `<head>` tags, add: `<script src="script.js"></script>`. Save and open your html - if it linked the two scripts together, it should give you a popup saying 'hello world!'! nice!

## The different parts of JS

Let's set up a basic JS function! Erase the `alert` from earlier and let's set up a function:


```
// this is a JS comment

var myVar = 0; // This is a variable 
// C++ users, notice how we don't have to declare the var type 

function myFunction() {
  myVar = myVar + 1; // equivalent to myVar++, if you want to be fancy!
  alert("Your variable is equal to: " + myVar);
}
```

Now, in your HTML in the `<body>`, add this:

```
<button onclick="myFunction()"> Click to call the function! </button>
```

See if it works! If it does, play around with the javascript and see what fun math you can do. +-/\* are all math operators.

Let's try a few more things. 

```
var myVar = 0; 

function myFunction(thing) {

  myVar = myVar + thing;
  
  document.getElementById('output').innerHTML = myVar;
}
```

HTML:

```
<button onclick="myFunction('i really love')">Add the text "i really love"</button>
<button onclick="myFunction('writing goddamn code!!!")>Add the text "writing some goddamn code"</button>
```


## Additional resources

If you want javascript to be useful, you're going to need a few libraries. Start by learning [Jquery](https://www.w3schools.com/JQuery/)
