# rime-misc
* 歡迎各位的反饋。

## 方案

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)。
* recommends:
  * [TRIME](https://github.com/osfans/trime)。
  * `"preset_keyboards/9key_terra_pinyin"`（本 repo）。
  * `dictgen_9key_stroke.schema.yaml`（五筆畫反查）（本 repo）。
* 多用簡拼就會開始卡頓。

### `9key_yytpiq_toneless` 9key_yytpiq_toneless
* \-

### `dictgen_9key_stroke` （9鍵反查用）五筆畫
* depends:
  * [`stroke.dict.yaml`](https://github.com/rime/rime-stroke)。
* recommends:
  * `9key_terra_pinyin.schema.yaml`（本 repo）。
* 必 deploy 之。

### `yytpiq_toneless` yytpiq_toneless
* 私人用……其他啲都已經 upload 嗮

## `~trime-keyboards.yaml`
* depends:
  * [TRIME](https://github.com/osfans/trime)。
* 要複製其內容到 `trime.custom.yaml`。
* 可以 swipe 空格鍵移動光標。`空格`+`swipe left / swipe right`→`move left / move right`。
  * 包括給 `preset_keyboards/qwerty` 和 `preset_keyboards/symbols` 的補丁，是爲此。（`a` 鍵難 swipe left……）

### `stroke` 五筆畫
* depends:
  * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke)。
* 沒有什麼特別
* <details><summary>截圖</summary><img alt="五筆畫" src="https://raw.githubusercontent.com/szc126/rime-misc/master/img/trime-stroke.png" /></details>

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * `9key_terra_pinyin.schema.yaml`（本 repo）。
* `PQRS`+`swipe left / swipe up / swipe down / swipe right`→`p / q / r / s`。
  * 可以之打全拼或全拼&middot;9鍵之混合。`5u\`→`路 lù`。
* <code>&#96;45678'</code>→`一丨丿丶乙`（五筆畫反查）。
* <details><summary>截圖</summary><img alt="9鍵地球拼音" src="https://raw.githubusercontent.com/szc126/rime-misc/master/img/trime-9key_terra_pinyin.png" /><img alt="9鍵地球拼音" src="https://raw.githubusercontent.com/szc126/rime-misc/master/img/trime-9key_terra_pinyin-stroke.png" /></details>

### `9key_yytpiq_toneless` 9key_yytpiq_toneless
* \-
* <details><summary>截圖</summary><img alt="9key_yytpiq_toneless" src="https://raw.githubusercontent.com/szc126/rime-misc/master/img/trime-9key_yytpiq_toneless.png" /></details>

### `qyeyshanglr_hanja` 옛한글・漢字
* depends:
  * [`qyeyshanglr_hanja.schema.yaml`](https://github.com/biopolyhedron/rime-qyeyshanglr-hanja)。
* `a`+`swipe right`→`ay`。
* `a`+`long click`→`ya`。
  * `a`+`swipe left`→`yay`。
* <details><summary>截圖</summary><img alt="옛한글・漢字" src="https://raw.githubusercontent.com/szc126/rime-misc/master/img/trime-qyeyshanglr_hanja.png" /></details>
