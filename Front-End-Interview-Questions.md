* Explain the concept of ES6 Promises to a 5-year-old.  
* What are the advantages of using ES6 maps over objects? What about using ES6 sets over arrays
* 	Given input:

// could be potentially more than 3 keys in the object above
items = [
{color: 'red', type: 'tv', age: 18},
{color: 'silver', type: 'phone', age: 20}
...
]

excludes = [
{k: 'color', v: 'silver'},
{k: 'type', v: 'tv'},
....
]
function excludeItems(items, excludes) {
   excludes.forEach(pair => {
      items = items.filter(item => item[pair.k] === item[pair.v]);
   });
   return items;
}

1. Describe what this function is doing...
2. What is wrong with that function ?
3. How would you optimize it ? https://www.glassdoor.co.in/Interview/Given-input-could-be-potentially-more-than-3-keys-in-the-object-above-items-color-red-type-tv-age-18-QTN_2372314.htm



* code an observer pattern
* Given 2 identical DOM trees (but not equal) and one element of the first DOM tree, how would you find this element in the second DOM tree?  
 * Write an array flatten function.  
* 	
No Offer
Positive Experience
Difficult Interview
Application

I applied through a recruiter. The process took 2+ months. I interviewed at Facebook (Menlo Park, CA (US)) in October 2016.

Interview

I applied through a recruiter who contacted me in September. She was nice and we booked a Phone/Screen coding interview.
They are using CoderPad for these. This first interview consisted of 3 questions, they all seemed pretty easy and then the interviewer asked for edge cases, a bit more challenging but nothing impossible. The interviewer was really nice and encouraging.
After that, I had another Phone/Screen interview which was basically the same.… 
Show More

Interview Questions

Given 2 identical DOM trees (but not equal) and one element of the first DOM tree, how would you find this element in the second DOM tree?  
3 Answers
Write an array flatten function.  
3 Answers
Write an emitter class:
/*
emitter = new Emitter();

// 1. Support subscribing to events.
sub = emitter.subscribe('event_name', callback);
sub2 = emitter.subscribe('event_name', callback2);

// 2. Support emitting events.
// This particular example should lead to the `callback` above being invoked with `foo` and `bar` as parameters.
emitter.emit('event_name', foo, bar);

// 3. Support unsubscribing existing subscriptions by releasing them.
sub.release(); // `sub` is the reference returned by `subscribe` above

* Can you write a function that deeply flattens an array?  
* some HTML and CSS design given a picture by the interviewer.  
* Given two identical DOM tree structures, A and B, and a node from A, find the corresponding node in B.  
* Given a picture, how would you hide/show a child picture on hovering on this parent?  
* How would you ensure clicking on this picture would go to a specific link?  
* How would you ensure the child is positioned in the top right of the parent picture?  
