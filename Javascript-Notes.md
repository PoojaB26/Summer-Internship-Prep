* Arrays are of reference type in JavaScript
* [When creating prototype object of reference type](https://gist.github.com/happymishra/0ba5ae121273e83c5883162f26410ee3#file-prototypeissue2-js)
* define all the object specific properties inside the constructor and all shared properties and methods inside the prototype
* [Prototypes](https://hackernoon.com/prototypes-in-javascript-5bba2990e04b)
* problem with using object literals (pre-ES6), is property/key orders are not guaranteed, \\all keys can only be strings.\\
Objects also lacks a forEach method. If you are used to iterating arrays using .forEach(), objects cannot be iterated in this way.
* Map provides a very convienent, .size property to get the size of the map.
* Another option to iterate the map is to use for..of syntax, which can easily provide access to the keys and values of the map.
```
for([key,value] of m) 
  console.log(key + '=' + value)
```
  
* m.keys() returns a full-blown iterator, so you can iterate the keys one by one, on demand, using .next()
* difference between map.values() and map.entries() => values return only the value, entries return an array of the kind [key, value]
* Maps can take 2d arrays in the constructor. Each array entry should have the format [key, value].
```
var arr = [['a', 1], ['b', 2]]
var m = new Map(arr)
```
* In set, you can *.add* same values.
* Difference between Arrays and sets : 
\\ Arrays -> contains whatever value you push
\\ Sets -> contains only unique values
* no primitive values can be added to WeakSet. It only accepts objects. No .forEach() to iterate
* According to Document Object Model (DOM), every HTML-tag is an object. Nested tags are called “children” of the enclosing one.
* The DOM represents HTML as a tree structure of tags.
* Tags are called element nodes (or just elements). Nested tags become children of the enclosing ones. \\
**As a result we have a tree of elements: <html> is at the root, then <head> and <body> are its children etc.**
* The text inside elements forms text nodes, labelled as #text. 
\\**A text node** contains only a string. It may not have children and **is always a leaf of the tree**.

* Everything in HTML, even comments, becomes a part of DOM.
* The reason we've put the <script> element near the bottom of the HTML file is that HTML is loaded by the browser in the order it appears in the file. If the JavaScript is loaded first and it is supposed to affect the HTML below it, it might not work, as the JavaScript would be loaded before the HTML it is supposed to work on. Therefore, putting JavaScript near the bottom of the HTML page is often the best strategy.
*  Document Object Model (DOM) API, allows you to manipulate documents.
* Everything in JavaScript is an object, and can be stored in a variable.
* Split and join functions
  ```
  var myData = 'Manchester,London,Liverpool,Birmingham,Leeds,Carlisle';
  var myArray = myData.split(',');
  var newString = myArray.join(',');

  ```
* All objects in JavaScript inherit from at least one other object. The object being inherited from is known as the prototype, and the inherited properties can be found in the prototype object of the constructor.

* Javascript has an interesting inheritance model, which happens to be completely different from most OOP languages. While it is object-oriented, an object doesn't have a type or a class that it gets its methods from, it has a prototype. The prototype of an object is a way to store common attributes across all instances of a class, but in a way that is overwritable. If an object doesn't have a reference to an attribute, that object's prototype will be checked for the attribute. https://community.risingstack.com/javascript-prototype-chain-inheritance/
* *this* is used inside a function, and will always refer to a single object — the object that invokes (calls) the function where “this” is used.
* in an IIFE like this:
```
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```
bar is declared inside an IIFE so its scope remains inside it, and cannot be outside the function. So second alert throughs a reference error.

* The z-index property specifies the stack order of an element. An element with greater stack order is always in front of an element with a lower stack order. Note: z-index only works on positioned elements (position:absolute, position:relative, or position:fixed).

