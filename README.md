# GravityBot Captcha

A simple npm package that will generate a random number in a captcha image for you!

## Features

- Based on `canvas-constructor/skia`
- Easy to use
- Medium difficulty against weak robots

## Requirement

- Node.js 16.x or higher
- [canvas-constructor](https://canvasconstructor.js.org)
- [skia-canvas](https://github.com/samizdatco/skia-canvas#readme)

## Installation

```npm
npm install @gravitybot/captcha
```

## Example usage

### Without number
```js
const { Captcha } = require('@gravitybot/captcha');

(async () => {

    const captcha = await new Captcha().create();

    console.log(captcha); // This should return a random number

})();
```

### With number
```js
const { Captcha } = require('@gravitybot/captcha');

(async () => {

    const captcha = await new Captcha().create(1976);

    console.log(captcha); // This should return the entred number '1976'

})();
```
