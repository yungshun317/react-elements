# React Elements

[![Made with JavaScript](https://img.shields.io/badge/Made_with-JavaScript-pink.svg)](https://img.shields.io/badge/Made_with-JavaScript-pink.svg) [![Powered by React](https://img.shields.io/badge/Powered%20by-React-lightblue)](https://img.shields.io/badge/Powered%20by-React-lightblue) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This project simply demonstrates how to use `React.createElement` and `ReactDOM.render`.

## Up & Running

Execute the `react-elements.html` with a browser, then you can see:
```sh
* 1 lb Salmon
* 1 cup Pine Nuts
* 2 cups Butter Lettuce
* 1 Yellow Squash
* 1/2 cup Olive Oil
* 3 cloves of Garlic
```

And the rendered HTML code looks like:
```html
<div id="react-container">
  <ul class="ingredients">
    <li>1 lb Salmon</li>
    <li>1 cup Pine Nuts</li>
    <li>2 cups Butter Lettuce</li>
    <li>1 Yellow Squash</li>
    <li>1/2 cup Olive Oil</li>
    <li>3 cloves of Garlic</li>
  </ul>
</div>
```

And the console log shows what `React.createElement` actually creates:
```json
{
    $$typeof: Symbol(react.element),
    "type": "ul"
    "key": null,
    "ref": null.
    "props": {
        "children": [
            { "type": "li", "props": { "children": "1 lb Salmon" } ... },
            { "type": "li", "props": { "children": "1 cup Pine Nuts" } ... },
            { "type": "li", "props": { "children": "2 cups Butter Lettuce" } ... },
            { "type": "li", "props": { "children": "1 Yellow Squash" } ... },
            { "type": "li", "props": { "children": "1/2 cup Olive Oil" } ... },
            { "type": "li", "props": { "children": "3 cloves of Garlic" } ... }
        ]
    },
    "_owner: null,
    "_store": { validated: false }
}
```

## React Elements

The virtual DOM is made up of React elements, which conceptually seem similar to HTML elements, but are actually JavaScript objects. It's much faster to work directly with JavaScript objects than it is to work with the DOM API. We make changes to a JavaScript object, the virtual DOM, and React renders those changes for us using the DOM API as efficiently as possible.

A React element is a description of what the actual DOM element should look like. In other words, React elements are the instructions for how the browser DOM should be created.

The major advantage of using React is its ability to separate data from UI elements.

## ReactDOM

ReactDOM contains the tools necessary to render React elements in the browser. We can render a React element, including its children, to the DOM with `ReactDOM.render`.

## Todos
 - Create full stack web applications with Spring Boot and React.

## License
[React Elements](https://github.com/yungshun317/react-elements) is released under the [MIT License](https://opensource.org/licenses/MIT) by [yungshun317](https://github.com/yungshun317).
