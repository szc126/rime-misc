# rime-misc
* 歡迎各位的反饋。

## 方案

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)。
* recommends:
  * [TRIME](https://github.com/osfans/trime)。
  * `preset_keyboards/9key_terra_pinyin`（本 repo）。
  * `dictgen_9key_stroke.schema.yaml`（五筆畫反查）（本 repo）。
* 多用簡拼就會開始卡頓。

### `9key_yytpiq_toneless` 9鍵三橛粵拼（無聲調）
* depends:
  * [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping)。
* recommends:
  * [TRIME](https://github.com/osfans/trime)。
  * `preset_keyboards/9key_yytpiq_toneless`（本 repo）。
  * `9key_terra_pinyin.schema.yaml`（拼音反查）（本 repo）。
* 麻煩。

### `16key_yytpiq_toneless` 16鍵三橛粵拼（無聲調）
* depends:
  * [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping)。
* recommends:
  * [TRIME](https://github.com/osfans/trime)。
  * `preset_keyboards/16key_yytpiq_toneless`（本 repo）。
  * `9key_terra_pinyin.schema.yaml`（拼音反查）（本 repo）。
* 應該唔會咁麻煩。

### `dictgen_9key_stroke` （9鍵反查用）五筆畫
* depends:
  * [`stroke.dict.yaml`](https://github.com/rime/rime-stroke)。
* recommends:
  * `9key_terra_pinyin.schema.yaml`（本 repo）。
* 必 deploy 之。

### `yytpiq_toneless` 三橛粵拼（無聲調）
* depends:
  * [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping)。
* recommends:
  * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)（拼音反查）。
    * OR [`luna_pinyin.dict.yaml`](https://github.com/rime/rime-luna-pinyin)（要自己修改）。
* 私人用……第啲都已經 upload 嗮

## `~trime-keyboards.yaml`
* depends:
  * [TRIME](https://github.com/osfans/trime)。
* 要複製其內容到 `trime.custom.yaml`。
* 可以 swipe 空格鍵移動光標。`空格`+`swipe left / swipe right`→`move left / move right`。
* `, / .` + 往空格鍵 swipe→`、 / ……`
* 鍵盤補丁：
  * `preset_keyboards/default`：改變 `Shift` `符號` `中文` 的排序爲 `中文` `符號` `Shift`
  * `a` 鍵難 swipe left，加 `空格`+`swipe left / swipe right`

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * `9key_terra_pinyin.schema.yaml`（本 repo）。
* `PQRS`+`swipe left / swipe up / swipe down / swipe right`→`p / q / r / s`。
  * 可以之打全拼、混打全拼&middot;9鍵。`5u\`→`路 lù`。
* <code>&#96;45678'</code>→`一丨丿丶乙`（五筆畫反查）。
* <details><summary>📷</summary><img alt="9鍵地球拼音" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_terra_pinyin-1_0_0.png" /><img alt="9鍵地球拼音" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_terra_pinyin-1_0_0-stroke.png" /></details>

### `9key_yytpiq_toneless` 9鍵三橛粵拼（無聲調）
* depends:
  * `9key_yytpiq_toneless.schema.yaml`（本 repo）。
* <details><summary>📷</summary><img alt="9鍵三橛粵拼（無聲調）" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_yytpiq_toneless-1_0_0.png" /><img alt="9鍵三橛粵拼（無聲調）" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_yytpiq_toneless-1_0_0-pinyin.png" /></details>

### `16key_yytpiq_toneless` 16鍵三橛粵拼（無聲調）
* depends:
  * `16key_yytpiq_toneless.schema.yaml`（本 repo）。
* <details><summary>📷</summary><img alt="16鍵三橛粵拼（無聲調）" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-16key_yytpiq_toneless-2_0_0.png" /></details>

### `qyeyshanglr_hanja` 옛한글・漢字
* depends:
  * [`qyeyshanglr_hanja.schema.yaml`](https://github.com/biopolyhedron/rime-qyeyshanglr-hanja)。
* `a`+`swipe right`→`ay`。
* `a`+`long click`→`ya`。
  * `a`+`swipe left`→`yay`。
* <details><summary>📷</summary><img alt="옛한글・漢字" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-qyeyshanglr_hanja-1_0_0.png" /></details>

### `stroke` 五筆畫
* depends:
  * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke)。
* 略改內裝的，沒有什麼特別
* <details><summary>📷</summary><img alt="五筆畫" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-stroke-1_0_0.png" /></details>
