# user-input-touch

![](https://travis-ci.org/apexearth/user-input-touch.svg)

Touch input state tracking, used by the `user-input` package.
Useful for game-loop style applications.

## Usage

[![NPM](https://nodei.co/npm/user-input-touch.png)](https://nodei.co/npm/user-input-touch/)

    var touch = window.touchInput(document)
    
    touch.touches        // Array of last touches.
    touch.changedTouches // Array of last changed touches.
    
## Tests

- Mocha
    - Test functionality in Node.js
    - `npm test`
- User Test
    - Test functionality in browser.
    - `npm user-test`
