# React swipeable views

> A React component for swipeable views

[![npm version](https://img.shields.io/npm/v/react-swipeable-views.svg?style=flat-square)](https://www.npmjs.com/package/react-swipeable-views)
[![npm downloads](https://img.shields.io/npm/dm/react-swipeable-views.svg?style=flat-square)](https://www.npmjs.com/package/react-swipeable-views)

Check out the [demos](http://oliviertassinari.github.io/react-swipeable-views/) from a mobile device (real or emulated).
It is tiny (<4kB) and quickly render the first slide then lasy-load the other.

## Installation

```sh
npm install --save react-swipeable-views
```

## Usage

```js
const React = require('react')
const SwipeableViews = require('react-swipeable-views')

const MyComponent = React.createClass({
    render: function () {
        return (
          <SwipeableViews>
            <div>
              slide n°1
            </div>
            <div>
              slide n°2
            </div>
            <div>
              slide n°3
            </div>
          </SwipeableViews>
        );
    }
});

module.exports = MyComponent;
```

## Props

- **index** Integer, *default=0* - This is the index of the slide to show.
This is useful when you want to change the default slide shown.
Or when you have tabs linked to each slide.

- **onChangeIndex** Function(index) - This is callback prop. It's call by the
component when the shown slide change after a swipe made by the user.
This is useful when you have tabs linked to each slide.

- **style** Object, *default={}* - This is the inlined style that will be apply
to each slide container.

## License

MIT
