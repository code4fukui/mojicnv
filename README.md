# mojicnv

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A simple web-based tool for converting between half-width (hankaku) and full-width (zenkaku) Japanese characters.

This project serves as a practical demonstration of the `HankakuKana.js` and `ZenkakuAlpha.js` modules from the [mojikiban](https://github.com/code4fukui/mojikiban) library by [Code for FUKUI](https://github.com/code4fukui/).

## Demo

**https://github.com/code4fukui/mojicnv

## Features

- Convert between half-width and full-width kana characters.
- Convert between half-width and full-width alphanumeric characters and symbols.

## Usage

The following examples demonstrate how to use the ES modules directly in your HTML.

### Half-Width ↔ Full-Width Kana

```js
import { HankakuKana } from "https://code4fukui.github.io/mojikiban/HankakuKana.js";

// Example: Convert input from one textarea to another on change
hankana.onchange = () => zenkana.value = HankakuKana.toZen(hankana.value);
zenkana.onchange = () => hankana.value = HankakuKana.toHan(zenkana.value);
```

### Half-Width ↔ Full-Width Alphanumerics & Symbols

```js
import { ZenkakuAlpha } from "https://code4fukui.github.io/mojikiban/ZenkakuAlpha.js";

// Example: Convert input from one textarea to another on change
hanalpha.onchange = () => zenalpha.value = ZenkakuAlpha.toZen(hanalpha.value);
zenalpha.onchange = () => hanalpha.value = ZenkakuAlpha.toHan(zenalpha.value);
```

## License

[MIT](LICENSE)