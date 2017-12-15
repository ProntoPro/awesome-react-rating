[![Build Status](https://travis-ci.org/ProntoPro/awesome-react-rating.svg?branch=master)](https://travis-ci.org/ProntoPro/awesome-react-rating)

# React Rating

React Rating is a [react](https://github.com/facebook/react) rating component built with `styled-components` [StyledComponent](https://github.com/styled-components/styled-components) 💅  and inspired by [ReactRating](https://github.com/dreyescat/react-rating/)

## Installation

You can install `awesome-react-rating` component using the *yarn* package manager:

```bash
yarn add --save @prontopro/awesome-react-rating
```

or *npm*:

```bash
npm install --save @prontopro/awesome-react-rating
```

### Dependencies

The `awesome-react-rating` component [peer depends](https://docs.npmjs.com/files/package.json#peerdependencies) on the [React](http://facebook.github.io/react/) library.

You can install React using *yarn* or *npm* too:

```bash
yarn add --save react
```

## Usage

1. Import Rating Component

    ```javascript
    import Rating from '@prontopro/awesome-react-rating'
    ```

2. Start using it

    Or with JSX:

    ```jsx
    <Rating />
    ```

## Properties

Property          | Type                                           | Default              | Description
---               | ---                                            | ---                  | ---
`start`           | *Number*                                       | 0                    | Range starting value.
`stop`            | *Number*                                       | 5                    | Range stop value.
`step`            | *Number*                                       | 1                    | Step increment (must be between *start* and *stop*).
`initialRate`     | *Number*                                       | 0                    | Initial rate value.
`emptyRate`       | *React Element*                                | Empty Star           | React Element
`fullRate`        | *React Element*                                | Full Star            | React element
`readonly`        | *Boolean*                                      | false                | Whether the rating can be modified or not.
`animateOnHover`  | *Boolean*                                      | false                | Whether to animate rate hovering or not.
`fractions`       | *Number*                                       | 1                    | Number of equal parts that make up a whole symbol.

## Callbacks

Callback      | Type                           | Description
---           | ---                            | ---
`onChange`    | rate => {}                     | Called when the selected rate is changed.
`onClick`     | (rate, event) => {}            | Called when a rate is clicked.
`onRate`      | rate => {}                     | Called when a rate is entered or left. When a rate is left it is called with `undefined`.

## License

[MIT License](https://github.com/ProntoPro/awesome-react-rating/blob/master/LICENSE.md)
