# mojicnv

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A set of character conversion tools.

## Demo
https://code4fukui.github.io/mojicnv/

## Features
- Convert between half-width and full-width kana characters
- Convert between half-width and full-width alphanumeric characters and symbols

## Usage

### Half-Width Kana ↔ Full-Width Kana

```js
import { HankakuKana } from "https://code4fukui.github.io/mojikiban/HankakuKana.js";

hankana.onchange = () => zenkana.value = HankakuKana.toZen(hankana.value);
zenkana.onchange = () => hankana.value = HankakuKana.toHan(zenkana.value);
```

### Full-Width Alphabet (Full-Width Symbols) ↔ Half-Width Alphabet (Half-Width Symbols)

```js
import { ZenkakuAlpha } from "https://code4fukui.github.io/mojikiban/ZenkakuAlpha.js";

hanalpha.onchange = () => zenalpha.value = ZenkakuAlpha.toZen(hanalpha.value);
zenalpha.onchange = () => hanalpha.value = ZenkakuAlpha.toHan(zenalpha.value);
```

## License
MIT License