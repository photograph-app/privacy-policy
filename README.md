# privacy-policy

Photograph が提供するアプリのプライバシーポリシー。GitHub Pages で公開し、Google Play とアプリから同じ URL を参照する(二重管理しない)。

## 構成

アプリごとにフォルダを作り、`index.md` に英語と日本語の本文を書く。言語ごとに `<div class="lang-section" lang="en" markdown="1">` で囲む(表示する言語だけを出すため)。フォルダ名はパッケージ名の最後の部分に合わせる。

| アプリ | フォルダ | 公開 URL |
| --- | --- | --- |
| Mosaic(`com.photograph.mosaic`) | `mosaic/` | https://photograph-app.github.io/privacy-policy/mosaic/ |

アプリを追加したら、`index.md` の一覧にも追加する。

## 変更する時

- 本文を変えたら、冒頭の最終更新日(英語・日本語の両方)も変える
- 公開 URL が変わると、Google Play に登録した URL とアプリ内のリンクが切れるため、フォルダ名は変えない
- Google Play Console の「データ セーフティ」の申告内容と食い違わないようにする

## 見た目

`_layouts/default.html` で決めている。

- URL に `?theme=dark` を付けて開いた時だけダークモードになる(アプリ内で表示する時に使う。ブラウザで普通に開いた時は明るいまま)
- 表示する言語は `?lang=en` / `?lang=ja` で指定する。指定が無ければブラウザの言語に合わせ、本文が無い言語は英語にする
- ブラウザで開いた時は右上の「Language」で切り替えられる(アプリから開いた時は端末の言語だけを表示し、切り替えは出さない)
- 言語を足す時は、本文に新しい言語の `lang-section` を足し、`default.html` の対応言語・選択肢・CSS にも追加する
