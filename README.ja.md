# mojicnv

日本語の半角文字と全角文字を相互に変換するシンプルなWebベースのツールです。

このプロジェクトは、[Code for FUKUI](https://github.com/code4fukui/)の[mojikiban](https://github.com/code4fukui/mojikiban)ライブラリに含まれる`HankakuKana.js`および`ZenkakuAlpha.js`モジュールの実践的なデモとして作成されています。

## デモ

**https://github.com/code4fukui/mojicnv

## 機能

- 半角カナと全角カナの相互変換
- 半角英数記号と全角英数記号の相互変換

## 使い方

以下の例は、HTML内で直接ESモジュールを使用する方法を示しています。

### 半角カナ ↔ 全角カナ

```js
import { HankakuKana } from "https://code4fukui.github.io/mojikiban/HankakuKana.js";

// 例: 変更時に一方のテキストエリアの入力を変換してもう一方に反映
hankana.onchange = () => zenkana.value = HankakuKana.toZen(hankana.value);
zenkana.onchange = () => hankana.value = HankakuKana.toHan(zenkana.value);
```

### 半角英数記号 ↔ 全角英数記号

```js
import { ZenkakuAlpha } from "https://code4fukui.github.io/mojikiban/ZenkakuAlpha.js";

// 例: 変更時に一方のテキストエリアの入力を変換してもう一方に反映
hanalpha.onchange = () => zenalpha.value = ZenkakuAlpha.toZen(hanalpha.value);
zenalpha.onchange = () => hanalpha.value = ZenkakuAlpha.toHan(zenalpha.value);
```

## ライセンス

[MIT](LICENSE)
