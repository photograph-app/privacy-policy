# privacy-policy

Photograph が提供するアプリのプライバシーポリシー。GitHub Pages で公開し、Google Play とアプリから同じ URL を参照する(二重管理しない)。

## 構成

アプリごとにフォルダを作り、`index.md` に英語と日本語の本文を書く。フォルダ名はパッケージ名の最後の部分に合わせる。

| アプリ | フォルダ | 公開 URL |
| --- | --- | --- |
| Mosaic(`com.photograph.mosaic`) | `mosaic/` | https://photograph-app.github.io/privacy-policy/mosaic/ |

アプリを追加したら、`index.md` の一覧にも追加する。

## 変更する時

- 本文を変えたら、冒頭の最終更新日(英語・日本語の両方)も変える
- 公開 URL が変わると、Google Play に登録した URL とアプリ内のリンクが切れるため、フォルダ名は変えない
- Google Play Console の「データ セーフティ」の申告内容と食い違わないようにする

## 見た目

`_layouts/default.html` で決めている。URL に `?theme=dark` を付けて開いた時だけダークモードになる(アプリ内で表示する時に使う。ブラウザで普通に開いた時は明るいまま)。
