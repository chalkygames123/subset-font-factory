# Japanese Font Subsetter

> Easy way to subset Japanese fonts

## Prerequisites

Make sure you have [Pipenv](https://pipenv.pypa.io/) installed.

## Setup

```shell
$ pipenv install
```

## Usage

Put the font files yout want to subset into the `src` directory and then run: `pipenv run ./make.sh`.

Note that by default the subsets include:

- All single-byte characters in Shift_JIS except control characters
- All double-byte characters in Shift_JIS except JIS level-2, level-3 and level-4 kanji

If you want to change this, edit the `chars.txt`.

## References

- [OpenTypeフォントの軽量化と自動カーニング - ureta.net](https://ureta.net/2017/02/tool_fonttools/)
- [文字コード表 シフトJIS(Shift_JIS)](http://charset.7jp.net/sjis.html)
- [JIS第1水準の漢字一覧表](http://kanjitisiki.com/jis1/)
- [ウェブフォントの最適化  |  Web Fundamentals  |  Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization)
