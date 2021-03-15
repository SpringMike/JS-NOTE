## InnerHTML

````javascript
var div1Element = document.querySelector('div:first-child > ul  ')
div1Element.innerHTML = '<li>Hello</li> <li>Hello</li> <li>Hello</li>'

//ghi de lai tat ca trong the ul = 3 the li
````

## OuterHTML

````javascript
var div3Element = document.querySelector('div:nth-child(2)> ul')

div3Element.innerHTML = '<h1>Hello</h1>'

//ghi de luon the ul = bang the h1
````



