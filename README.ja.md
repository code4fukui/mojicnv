# mojicnv

文字変換ツールのコレクションです。半角カナと全角カナ、全角アルファベットと半角アルファベットの相互変換が可能です。

## 機能
- 半角カナと全角カナの変換
- 全角アルファベットと半角アルファベットの変換

## 使い方

### 半角カナ⇔全角カナ

```js
import { HankakuKana } from "https://code4fukui.github.io/mojikiban/HankakuKana.js";

hankana.onchange = () => zenkana.value = HankakuKana.toZen(hankana.value);
zenkana.onchange = () => hankana.value = HankakuKana.toHan(zenkana.value);
```

### 全角アルファベット⇔半角アルファベット

```js
import { ZenkakuAlpha } from "https://code4fukui.github.io/mojikiban/ZenkakuAlpha.js";

hanalpha.onchange = () => zenalpha.value = ZenkakuAlpha.toZen(hanalpha.value);
zenalpha.onchange = () => hanalpha.value = ZenkakuAlpha.toHan(zenalpha.value);
```

## ライセンス
MIT