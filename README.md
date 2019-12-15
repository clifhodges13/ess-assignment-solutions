# ESS Frontend Assignment
Develop two solutions that are cross-platform compatible and delivers the same functionality and styling that exists in the index.html page without the use of an iframe. 

## Getting Started
1. open index.html in an iframe supported browser to be able to see the iframe's content (ex: Chrome)
2. Code away!

## Requirements
* Come up with two solutions to solve this problem. 
* In the included README.md please include a brief explanation as to why each solution was chosen.
* ** The index.html styling should only be dependent on the main.css file. **
* ** The content that was previously rendered by the iframe should not be affected by the main.css file but should still have styling. **
* The solutions should be compatible across all browsers (Edge, IE, Chrome, Firefox, Mobile)


## For each solution please provide a brief explanation below.

## Explanations

HTML Object:
  * By using an HTML object with an HTML embed, we can embed external pages into our page without the use of an iframe. The tricky part was having access to the DOM elements inside of the embedded page from the index.html. I was able to change the contents of the embed by updating the src attribute when the navBtn was clicked. The HTML object and embed are supported in all browsers, including Internet Explorer.

React Application:
  * I chose to build this solution using a React application because of the maintainability and reusability. The create-react-app, used to bootstrap this application also comes with out-of-the-box cross-browser compatibility. Because React works with the Virtual DOM, it only rerenders those components whose state changes. This prevents an entire page refresh after every user request.
  * Styled components were used here to separate the styles.
  * Run `npm start` to boot up the local server and view the solution in your browser.