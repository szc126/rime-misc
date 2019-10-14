# rime-misc
* 歡迎各位的反饋。

## Schemas

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin).
* recommends:
  * [TRIME](https://github.com/osfans/trime).
  * `preset_keyboards/9key_terra_pinyin` (this repo).
  * `dictgen_9key_stroke.schema.yaml` (五筆畫 reverse lookup) (this repo).

### `9key_yytpiq_toneless` 9鍵三橛粵拼（無聲調）
* depends:
  * [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping).
* recommends:
  * [TRIME](https://github.com/osfans/trime).
  * `preset_keyboards/9key_yytpiq_toneless` (this repo).
  * `9key_terra_pinyin.schema.yaml` (拼音 reverse lookup) (this repo).

### `16key_yytpiq_toneless` 16鍵三橛粵拼（無聲調）
* depends:
  * [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping).
* recommends:
  * [TRIME](https://github.com/osfans/trime).
  * `preset_keyboards/16key_yytpiq_toneless` (this repo).
  * `9key_terra_pinyin.schema.yaml` (拼音反查) (this repo).

### `dictgen_9key_stroke` （9鍵反查用）五筆畫
* depends:
  * [`stroke.dict.yaml`](https://github.com/rime/rime-stroke).
* recommends:
  * `9key_terra_pinyin.schema.yaml` (this repo).
* You must deploy it, in order to create the Prism.

### `yytpiq_toneless` 三橛粵拼（無聲調）
* depends:
  * [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping).
* recommends:
  * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin) (拼音 reverse lookup).
    * or [`luna_pinyin.dict.yaml`](https://github.com/rime/rime-luna-pinyin) (you must change this yourself).
* my personal shit

## TRIME keyboards
* depends:
  * [TRIME](https://github.com/osfans/trime).
* `space`+`swipe left`→`move left`. `space`+`swipe right`→`move right`.
* `,` + swipe towards `space`→`、`. `.` + swipe towards `space`→`……`.

```
patch:
  __include: ~trime.custom.keyboard.qyeyshanglr_hanja:/
  __include: ~trime.custom.space_swipe:/
```
* ([Configuration &middot; rime/home Wiki](https://github.com/rime/home/wiki/Configuration))

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * `9key_terra_pinyin.schema.yaml` (this repo).
* `PQRS`+`swipe left / swipe up / swipe down / swipe right`→`p / q / r / s`.
  * You can use this to type 全拼, or mixed 全拼-T9. `5u\`=`lù`.
* <code>&#96;45678'</code>→`一丨丿丶乙` (五筆畫 reverse lookup).
* <details><summary>📷</summary><img alt="9鍵地球拼音" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_terra_pinyin-1_0_0.png" /><img alt="9鍵地球拼音" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_terra_pinyin-1_0_0-stroke.png" /></details>

### `9key_yytpiq_toneless` 9鍵三橛粵拼（無聲調）
* depends:
  * `9key_yytpiq_toneless.schema.yaml` (this repo).
* <details><summary>📷</summary><img alt="9鍵三橛粵拼（無聲調）" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_yytpiq_toneless-1_0_0.png" /><img alt="9鍵三橛粵拼（無聲調）" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_yytpiq_toneless-1_0_0-pinyin.png" /></details>

### `16key_yytpiq_toneless` 16鍵三橛粵拼（無聲調）
* depends:
  * `16key_yytpiq_toneless.schema.yaml` (this repo).
* <details><summary>📷</summary><img alt="16鍵三橛粵拼（無聲調）" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-16key_yytpiq_toneless-2_0_0.png" /></details>

### `qyeyshanglr_hanja` 옛한글・漢字
* depends:
  * [`qyeyshanglr_hanja.schema.yaml`](https://github.com/biopolyhedron/rime-qyeyshanglr-hanja).
* `a`+`swipe right`→`ay`.
* `a`+`long click`→`ya`.
  * `a`+`swipe left`→`yay`.
* <details><summary>📷</summary><img alt="옛한글・漢字" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-qyeyshanglr_hanja-1_0_0.png" /></details>

### `stroke` 五筆畫
* depends:
  * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke).
* 改悪・私的用。
* <details><summary>📷</summary><img alt="五筆畫" src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-stroke-1_0_0.png" /></details>

## TRIME keyboards: patches

### `number_controls`

### `rearrange_default`

### `space_swipe`
