# mojicnv
 
https://code4fukui.github.io/mojicnv/

## Usage

### 半角カナ←→全角カナ

```js
import { HankakuKana } from "https://code4fukui.github.io/mojikiban/HankakuKana.js";

hankana.onchange = () => zenkana.value = HankakuKana.toZen(hankana.value);
zenkana.onchange = () => hankana.value = HankakuKana.toHan(zenkana.value);
```

### 全角アルファベット（全角記号英数）←→半角アルファベット（半角記号英数）

```js
import { ZenkakuAlpha } from "https://code4fukui.github.io/mojikiban/ZenkakuAlpha.js";

hanalpha.onchange = () => zenalpha.value = ZenkakuAlpha.toZen(hanalpha.value);
zenalpha.onchange = () => hanalpha.value = ZenkakuAlpha.toHan(zenalpha.value);
```
