
### 1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

getElementById → uses its id to select one element.
  getElementsByClassName→ selects all elementsthat belong to the same class.
  querySelector → selects the first element that corresponds to a CSS selector.
  querySelectorAll → selects all elements that fit a CSS selector.

### 2. How do you create and insert a new element into the DOM?
1. To create a new element, use    document.createElement().
2. Include content (such as HTML or text) in it.
3. Select the parent element to insert it into.
4. Insert the new element inside the parent using appendChild()
### 3. What is Event Bubbling? And how does it work?

  When an element  is clicked, the event begins there and then "bubbles up" to its parent, then its grandparent, and finally the document.

A child element is clicked.The child is the first to experience the event.
After that, its parent, the parent's parent, and so on automatically experience the same thing.Until it reaches the top of the DOM , this keeps happening.
### 4. What is Event Delegation in JavaScript? Why is it useful?
We add it to the parent rather than adding an event listener to each child element.
  Advantages:
 1. Preserves memory
   2.Simplifies code
  3.Automatically manages new child elements
### 5. What is the difference between preventDefault() and stopPropagation() methods?
preventDefault() → halts an element's default action.
  stopPropagation() → prevents the event from bubbling up to parent elements.