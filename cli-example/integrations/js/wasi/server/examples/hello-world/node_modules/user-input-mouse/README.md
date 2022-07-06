# user-input-mouse

![](https://travis-ci.org/apexearth/user-input-mouse.svg)
![](http://img.shields.io/npm/v/user-input-mouse.svg?style=flat)
![](http://img.shields.io/npm/dm/user-input-mouse.svg?style=flat)
![](http://img.shields.io/npm/l/user-input-mouse.svg?style=flat)

Stores the latest state values received from mouse events.

## Install

[![NPM](https://nodei.co/npm/user-input-mouse.png)](https://nodei.co/npm/user-input-mouse/)

### Usage

    var mouse = window.mouseInput(document)

When the user presses the left mouse button at coordinates (x100,y200), `mouse` would contain the following.

    {
        "x": 100,
        "y": 200,
        "mouse0": 1
    }

When the user releases the left mouse button at (x110,y200), and then presses the right mouse button at (x200,y300), `mouse` would contain the following.

    {
        "x": 200,
        "y": 300,
        "mouse0": 0,
        "mouse2": 1
    }

The values shown always represent the latest values received.

## Tests

- Mocha
    - Test functionality in Node.js
    - `npm test`
- User Test
    - Test functionality in browser.
    - `npm run user-test`
