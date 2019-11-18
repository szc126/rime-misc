# rime-misc
* 歡迎各位的反饋。

## Schemas

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)
* recommends:
  * [TRIME](https://github.com/osfans/trime)
  * `preset_keyboards/9key_terra_pinyin` (this repo)
  * reverse lookup: `dictgen_9key_stroke.schema.yaml` (this repo)

### `9key_yytpiq` 9鍵三橛粵拼
* depends:
  * [`jyut6ping3.dict.yaml`](https://github.com/sgalal/rime-cantonese)
    * or [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping)
* recommends:
  * [TRIME](https://github.com/osfans/trime)
  * `preset_keyboards/9key_yytpiq` (this repo)
  * reverse lookup: `9key_terra_pinyin.schema.yaml` (this repo)

### `16key_yytpiq` 16鍵三橛粵拼
* depends:
  * [`jyut6ping3.dict.yaml`](https://github.com/sgalal/rime-cantonese)
    * or [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping)
* recommends:
  * [TRIME](https://github.com/osfans/trime)
  * `preset_keyboards/16key_yytpiq` (this repo)
  * reverse lookup: `9key_terra_pinyin.schema.yaml` (this repo)

### `dictgen_9key_stroke` （9鍵反查用）五筆畫
* depends:
  * [`stroke.dict.yaml`](https://github.com/rime/rime-stroke)
* recommends:
  * `9key_terra_pinyin.schema.yaml` (this repo)
* description:
  * You must deploy this schema and create `dictgen_9key_stroke.prism.bin`.

### `yytpiq` 三橛粵拼
* depends:
  * [`jyut6ping3.dict.yaml`](https://github.com/sgalal/rime-cantonese)
    * or [`jyutping.dict.yaml`](https://github.com/rime/rime-jyutping)
* recommends:
  * reverse lookup: [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)
    * or [`luna_pinyin.dict.yaml`](https://github.com/rime/rime-luna-pinyin)
* description:
  * my personal shit

## TRIME keyboards
* depends:
  * [TRIME](https://github.com/osfans/trime)
* description:
  * `space`+`swipe left`→`move left`. `space`+`swipe right`→`move right`
  * `,` + swipe towards `space`→`、`. `.` + swipe towards `space`→`……`

```
patch:
  __include: ~trime.custom.keyboard.qyeyshanglr_hanja:/
  __include: ~trime.custom.space_swipe:/
```
* ([Configuration &middot; rime/home Wiki](https://github.com/rime/home/wiki/Configuration))

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * `9key_terra_pinyin.schema.yaml` (this repo)
* <details>
    <summary>📷</summary>
    <img
      alt="9鍵地球拼音"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_terra_pinyin-1_0_0.png"
    />
    <img
      alt="9鍵地球拼音"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_terra_pinyin-1_0_0-stroke.png"
    />
  </details>

### `9key_yytpiq` 9鍵三橛粵拼
* depends:
  * `9key_yytpiq.schema.yaml` (this repo)
* <details>
    <summary>📷</summary>
    <img
      alt="9鍵三橛粵拼"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_yytpiq-1_0_0.png"
    />
    <img
      alt="9鍵三橛粵拼"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-9key_yytpiq-1_0_0-pinyin.png"
    />
  </details>

### `16key_yytpiq` 16鍵三橛粵拼
* depends:
  * `16key_yytpiq.schema.yaml` (this repo)
* <details>
    <summary>📷</summary>
    <img
      alt="16鍵三橛粵拼"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-16key_yytpiq-2_0_0.png"
    />
  </details>

### `qyeyshanglr_hanja` 옛한글・漢字
* depends:
  * [`qyeyshanglr_hanja.schema.yaml`](https://github.com/biopolyhedron/rime-qyeyshanglr-hanja)
* description:
  * iotation:
    * `a`+`long click`→`ya`
      * `a`+`swipe left`→`yay`
    * `a`+`swipe right`→`ay`
* <details>
    <summary>📷</summary>
    <img
      alt="옛한글・漢字"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-qyeyshanglr_hanja-1_0_0.png"
    />
  </details>

### `stroke` 五筆畫
* depends:
  * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke)
* description:
  * 改悪
  * 私的用
* <details>
    <summary>📷</summary>
    <img
      alt="五筆畫"
      src="https://raw.githubusercontent.com/szc126/rime-misc/img/img/trime-stroke-1_0_0.png"
    />
  </details>

## TRIME keyboards: patches

### `number_controls`

### `rearrange_default`

### `space_swipe`
