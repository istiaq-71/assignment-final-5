# assignment-final-5


1. Difference between `getElementById`, `getElementsByClassName`, and `querySelector` / `querySelectorAll`?

- `getElementById`**: Grabs one element by its unique `id`. Returns that element or nothing if no match.
- `getElementsByClassName`**: Gets all elements with a specific class. Gives a live list that updates if the page changes.
- `querySelector`**: Picks the first element matching a CSS selector (like `#id`, `.class`, or `tag`). Super flexible.
- `querySelectorAll`**: Gets all elements matching a CSS selector. Returns a static list you can loop through.

Difference: `getElementById` is for one `id`, `getElementsByClassName` is for classes, and `querySelector`/`querySelectorAll` work with any CSS selector. First two are faster but less flexible.



2. How to create and insert a new element into the DOM?

- Create an element with `document.createElement("tag")` (like `"div"` or `"p"`).
- Add stuff like text, classes, or IDs to it if needed.
- Attach it to the page using methods like `appendChild`, `append`, or `prepend` to a parent element (like a `div` with an `id`).



3. What is Event Bubbling and how does it work?

Event bubbling is when an event (like a click) on an element triggers on that element first, then moves up to its parent, then the parent’s parent, all the way to the top of the page. It’s like ripples spreading outward.



4. What is Event Delegation in JavaScript? Why is it useful?

Event delegation is putting one event listener on a parent element to handle events for its children, using bubbling. You check which child was clicked using `event.target`.

Why useful**: Saves memory (fewer listeners), works for new elements added later, and makes code simpler.



5. Difference between `preventDefault()` and `stopPropagation()`?

- `preventDefault()`: Stops the browser’s default action (like a link navigating or form submitting).
- `stopPropagation()`: Stops the event from moving up to parent elements (or down in rare cases).

Difference: `preventDefault` blocks what the element normally does; `stopPropagation` keeps the event from affecting other elements.
