#  Attribute

## example

````javascript
var h1Element = document.querySelector('h1')

h1Element.title ='Học lập trình tại F8'

var divElement = document.querySelector('div')

divElement.className = 'box'

var widthElement = document.querySelector('img')

widthElement.width = 100
````

## getAttribute()

````javascript
var x = document.querySelector("h1")[0].getAttribute("class");

var f8ShortLink = f8LinkElement.getAttribute('href')
````

## setAttribute()

````javascript
document.querySelectorAll('a')[1].setAttribute('href',f8ShortLink)


document.querySelector('div').setAttribute('data-url',f8ShortLink)
````

