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

