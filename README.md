# Constructors

Build webpages without a templating engine in fewer lines of code. This is useful for Chrome extensions that need to add content to pages.

**Example**
```js
1. var h1 = new DivElem({ appendTo: document.body, type: 'h1', txt: 'Hello', clss: 'text-center', clck: function() { console.log('Hello'); } });
```
The code above creates a `h1` element, appends it to the document body, gives it the text 'Hello', and adds an event listener for click. Compare it to the same accomplishment below:
```js
1. var h1 = document.createElement('h1');
2. h1.innerText = 'Hello';
3. h1.className = 'text-center';
4. h1.addEventListener('click', function() {
5.     console.log('Hello');
6. });
7. document.body.appendChild(h1);```
