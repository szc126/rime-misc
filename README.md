# rime-misc
* 歡迎各位的反饋。

## 配方

### `9key_terra_pinyin` 9鍵地球拼音
* TRIME用。
* 多用簡拼就會開始卡頓。
* 要 [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)。
* 建議安裝 `dictgen_9key_stroke.schema.yaml`（反查）。

### `dictgen_9key_stroke` （9鍵反查用）五筆畫
* 是爲了`9key_terra_pinyin`的五筆畫反查。必 deploy 之。
* 要 [`stroke.dict.yaml`](https://github.com/rime/rime-stroke)。

### `yytpiq_toneless` yytpiq_toneless
* 私人用……其他啲都已經 upload 嗮

### `~trime_keyboards.yaml`
* TRIME用。要複製其內容到 `trime.custom.yaml`。
* 可以 swipe 空格鍵移動光標。`空格`+`swipe left / swipe right`→`move left / move right`。

#### `stroke` 五筆畫
* \-

#### `9key_terra_pinyin` 9鍵地球拼音
* `PQRS`+`swipe left / swipe up / swipe down / swipe right`→`p / q / r / s`。
  * 可以之打全拼或全拼&middot;9鍵之混合。`5u\`→`路 lù`。
* <code>&#96;45678'</code>→`一丨丿丶乙`（五筆畫反查）。

#### `qyeyshanglr_hanja` 옛한글・漢字
* `a`+`swipe right`→`ay`。
* `a`+`long click`→`ya`。
  * `a`+`swipe left`→`yay`。
