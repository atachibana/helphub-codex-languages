# HelpHub Codex Languages

WordPress plugin HelpHub Codex Languages provides shortcode for HelpHub languages link. It is based on Codex language link.

Language link in Codex is
```
{{Languages|
{{en|Administration Screens}}
{{fr|Panneaux Administration}}
{{ja|管理画面}}
}}
```
can be converted to as like as below in HelpHub:
```
[codex_languages en="Administration Screens" ja_codex="管理画面" fr_codex="Panneaux Administration"]
```
## Supported locales

Refer reamde.txt

### Notice for pt-br, zh-cn and zh-tw

In language parameter, 51 locales are supported as usual language symbol such as 'en', 'fr', 'ja', etc. except 'pt-br', 'zh-cn' and 'zh-tw'.

By unknown reason, shortcode cannot handle hyphen character well and ignored the parameter. Above language locale that includes hyphen in it, must be specified without hypen such as 'ptbr', 'zhcn' and 'zhtw'.

## 'xy' vs. 'xy_codex'

Current locale symbol has '\_codex' suffix. For example French is 'fr_codex', not 'fr'. This is because simpler locale symbol was reserved for the symbol for the internationalized HelpHub.

## Original repository

Originally this branch was clone of HelpHub. For older commits than 10/Aug/2016, refer below branch.

Original repoistory: https://github.com/atachibana/HelpHub

Branch: https://github.com/atachibana/HelpHub/tree/Short-code-codex_languages

# Files

```
README.md                         readme (This file)
helphub-codex-languagex.php       plugin
index.php                         dummy
readme.text                       readme for plugin

assets/
  css/
    codex-languages.css           stylesheet
```

# Author
Akira Tachibana (http://unofficialtokyo.com)

# History

## Version 2.0 (10/Aug/2016)
* Plugin
https://github.com/atachibana/HelpHub/commit/b0a773ccfc7320d9cc93678344c3b1117a3361c9

## Version 1.1 (8/Aug/2016)
* Suffix "\_codex" were added.
* Hypen character in language code caused an issue in Shortcode.
* Not plugin

By Rami's suggestion, suffix "\_codex" are appended to each short code symbol, because simple language locator should be kept for the future final goal style.
The hyphen character should be avoided in short code because some troble occurred.  pt-br, zh-cn, zh-tw are changed to ptbr, zhcn, zhcw.
https://github.com/atachibana/HelpHub/commit/5b0de101042e0efc2c7f9bf62ad84775b9fd3dee

## Version 1.0 (2/Aug/2016)
* Initial
* Not plugin. functions.php embedded version.
https://github.com/atachibana/HelpHub/commit/068e2c343e6435680fb89d9418e6483145864a77
