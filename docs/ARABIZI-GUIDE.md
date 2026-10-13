# Arabic romanised input in Lambe

Choose **Arabic · Arabizi (McGovern-based)** in Writing mode. The input starts empty. The mode is included in this app and can also be imported from `arabic-romanized-lambe.json`.

For an independent copy, use **Create your own mode**, select the existing Arabic mode in **Start from**, and save it with a distinct name. Alternatively, choose **Import mode** and open `arabic-romanized-lambe.json`. Import gives the copy its own identifier.

## Numbers used as letters

| Input | Arabic | Tengwa in this mode |
|---|---|---|
| `2` | ء | Calma |
| `3` | ع | Anga |
| `3'`, `gh` | غ | Unque |
| `5`, `7'`, `kh` | خ | Hwesta |
| `6` | ط | Extended tinco |
| `6'` | ظ | Extended anga |
| `7` | ح | Vilya |
| `8`, `q` | ق | Extended quessë |
| `9` | ص | Extended calma |
| `9'` | ض | Extended ando |

Straight and curly apostrophes work in the digit combinations. `ʿ` and `ʕ` are also accepted for ʿayn; a standalone apostrophe or `ʾ` denotes hamza. Latin input is case-insensitive: use `9`, not capital `S`, to distinguish ṣād from sīn.

The other consonant spellings are `b t th j d dh r z s sh f k l m n h w y`. `dj` also denotes jīm; `x` denotes khāʾ. Academic spellings such as `ḥ ṣ ḍ ṭ ẓ ġ ḫ ṯ ḏ` are accepted. Ambiguous `g` and `ch` remain visible Latin text until you define their intended values in the mode editor.

This profile assigns `8` to qāf and `9` to ṣād. Other communities use different conventions. It treats `2` as the pronounced glottal stop, including when that sound corresponds to qāf in a dialect; it does not reconstruct the original Arabic spelling.

## Vowels and spelling

| Input | Value | Result |
|---|---|---|
| `a` | short /a/ | Three dots above the preceding consonant |
| `i`, `e` | short /i/ | Dot above the preceding consonant |
| `u`, `o` | short /u/ | Right curl above the preceding consonant |
| `aa`, `ā`, `â` | long /aː/ | Short carrier with three dots |
| `ii`, `ee`, `ī`, `î` | long /iː/ | Yanta |
| `uu`, `oo`, `ū`, `û` | long /uː/ | Úrë |

A short vowel at the beginning of a word gets a carrier. Spell consonantal /w/ as `w` and /j/ as `y`. Write diphthongs as `aw` and `ay`.

`e/ee` and `o/oo` are convenience spellings of the i/u vowels in this profile. They do not define separate dialectal /e/ and /o/ phonemes. To distinguish those sounds, change or add associations in your own copy.

Repeat the complete consonant token to indicate gemination: `bb`, `ll`, `shsh`, `khkh`, or `3'3'`. The result is one consonant with a doubling bar below. For example, `mu7ammad` applies this to the doubled mīm.

Explicit optional spellings are `t*` for tāʾ marbūṭa, `a*` for alif maqṣūra, and `a~`, `i~`, `u~` for tanwīn. The mode does not infer these from word endings. `laa` and `lā` use the lam–alif form. Hamza uses the independent calma form consistently; this input mode does not choose Arabic hamza seats.

## Literal numbers

In this mode, unescaped digit inputs are letters wherever they are defined. To enter an actual number, put one backslash before the complete run:

```text
\2026
\123
```

The backslash is an input control and is not drawn. **Tengwar numerals** changes these number runs between ordinary and Tengwar numerals; it never changes `3` as ʿayn or `7` as ḥāʾ. Digits without letter associations (`0`, `1`, `4`) remain numbers without an escape as well.

Spaces and empty lines are preserved. Unknown characters remain visible. You can adjust every resulting tengwa and tehta through the existing positioning controls.

## Examples

```text
3arabi
7abibi
7abiibi
mu7ammad
salaam
```

These are examples to type yourself; none is loaded into the input automatically.

## Basis and compatibility

The consonant assignments and basic vowel signs follow Gabriel McGovern's 2016 Arabic Tengwar charts. The Arabizi aliases, explicit input controls and consistent independent-hamza policy are Lambe adaptations. This is a usable McGovern-based romanised input mode, not a claim to reproduce every orthographic detail of the original system or to standardise all Arabic dialects.

Sources: [McGovern's mode and charts](https://www.omniglot.com/conscripts/taynwaat.htm), [the chart spreadsheet](https://www.omniglot.com/charts/tengwar_arabic.xls), and [GulfArabic's Arabizi conventions](https://www.gulfarabic.com/a12_arabiizi_chat_arabic.php).

The JSON uses Lambe's schema version 1. Digit inputs require the updated Windows or Android engine in Lambe 0.9.6 or later; the earlier Flutter 0.9.5 engine handles digits before associations. This profile is included in both apps and can be exported or duplicated. All inputs and previews start blank.
