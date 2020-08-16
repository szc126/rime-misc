# rime-misc
* 歡迎各位的反饋。
* screenshots: https://gist.github.com/szc126/826a3b059bf092b12e990c06448e19f8

## Schemas

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * dictionary:
    * [`terra_pinyin.dict.yaml`](https://github.com/rime/rime-terra-pinyin)
* recommends:
  * [TRIME](https://github.com/osfans/trime)
  * keyboard layout:
    * `preset_keyboards/9key_terra_pinyin` (this repo)
  * reverse lookup:
    * `dictgen_9key_stroke.schema.yaml` (this repo)

### `9key_yytpiq` 9鍵三橛粵拼
* depends:
  * dictionary:
    * [`jyut6ping3.dict.yaml`](https://github.com/sgalal/rime-cantonese)
* recommends:
  * [TRIME](https://github.com/osfans/trime)
  * keyboard layout:
    * `preset_keyboards/9key_yytpiq` (this repo)
  * reverse lookup:
    * `9key_terra_pinyin.schema.yaml` (this repo)
    * `dictgen_9key_stroke.schema.yaml` (this repo)

### `16key_yytpiq` 16鍵三橛粵拼
* depends:
  * dictionary:
    * [`jyut6ping3.dict.yaml`](https://github.com/rime/rime-cantonese)
* recommends:
  * [TRIME](https://github.com/osfans/trime)
  * keyboard layout:
    * `preset_keyboards/16key_yytpiq` (this repo)
  * reverse lookup:
    * [`terra_pinyin.schema.yaml`](https://github.com/rime/rime-terra-pinyin)
    * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke)

### `dictgen_9key_stroke` （9鍵反查用）五筆畫
* depends:
  * dictionary:
    * [`stroke.dict.yaml`](https://github.com/rime/rime-stroke)
* description:
  * You must deploy this schema and create `dictgen_9key_stroke.prism.bin`.

### `yytpiq` 三橛粵拼
* depends:
  * dictionary:
    * [`jyut6ping3.dict.yaml`](https://github.com/rime/rime-cantonese)
* recommends:
  * reverse lookup:
    * [`terra_pinyin.schema.yaml`](https://github.com/rime/rime-terra-pinyin)
    * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke)
* description:
  * personal schema
  * why do i have to give things names

## TRIME keyboards
* depends:
  * [TRIME](https://github.com/osfans/trime)
* description:
  * `space`+`swipe left`→`move left`
  * `space`+`swipe right`→`move right`
  * `,` + swipe towards `space`→`、`
  * `.` + swipe towards `space`→`……`

```
patch:
  __include: ~trime.custom.keyboard.9key_terra_pinyin:/
  __include: ~trime.custom.space_swipe:/
```
* ([Configuration &middot; rime/home Wiki](https://github.com/rime/home/wiki/Configuration))

### `9key_terra_pinyin` 9鍵地球拼音
* depends:
  * `9key_terra_pinyin.schema.yaml` (this repo)

### `9key_yytpiq` 9鍵三橛粵拼
* depends:
  * `9key_yytpiq.schema.yaml` (this repo)

### `16key_yytpiq` 16鍵三橛粵拼
* depends:
  * `16key_yytpiq.schema.yaml` (this repo)

### `qyeyshanglr_hanja` 옛한글・漢字
* depends:
  * [`qyeyshanglr_hanja.schema.yaml`](https://github.com/biopolyhedron/rime-qyeyshanglr-hanja)
* description:
  * iotation:
    * `a`+`long click`→`ya`
      * `a`+`swipe left`→`yay`
    * `a`+`swipe right`→`ay`

### `stroke` 五筆畫
* depends:
  * [`stroke.schema.yaml`](https://github.com/rime/rime-stroke)
* description:
  * 改悪
  * 私用

## TRIME keyboards: patches

### `number_controls`

### `rearrange_default`

### `space_swipe`
