# DOM get() method



## querySelector() & querySelectorAll()



````javascript
document.querySelector(".example");

document.querySelector("p");

document.querySelector("p.example");

document.querySelector("a[target]");
//Get the first <a> element in the document that has a "target" attribute:

var listItems1 = document.querySelectorAll('.parent>li')

var listItems2 = document.querySelectorAll('.parent> ul > li')

document.querySelector("h2, h3")

var x = document.querySelectorAll(".example");
````



## getElementsByClassName()



````javascript
var x = document.getElementsByClassName("example");

var boxHTMLCollection = document.getElementsByClassName('box')


var box2Element = document.getElementsByClassName('box')[1]

var box1ItemElements = document.getElementsByClassName('box')[0].getElementsByClassName('item')
var box2ItemElements = 
    
document.getElementsByClassName('box')[1].getElementsByClassName('item')
````



## getElementsByTagName



````javascript
var x = document.getElementsByTagName("LI");
````



## getElementById



```javascript
document.getElementById("demo");
```

