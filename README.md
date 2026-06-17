# game-demand-forecast-slides

## 概要

[game-demand-forecast](https://github.com/rindguitar/game-demand-forecast)（ゲーム需要予測システム）の発表用スライドです。

Steam APIのデータを使い、NLP・時系列分析でプレイヤーが求めるゲーム要素・トレンドを予測するプロジェクトを紹介します。

## 開発環境

[reveal.js](https://github.com/hakimel/reveal.js) によってスライドを作成しています。
Node.js, npmが利用できる環境で、以下のコマンドで開発環境の構築ができます:

```bash
npm install
```

## 使い方

### スライド作成

以下のコマンドでローカルサーバーを起動:

```bash
npm start
```

ブラウザで [http://localhost:8000](http://localhost:8000) にアクセスすると、スライドをプレビューできます。

スライドの内容は [`index.html`](index.html) の Markdown を編集してください。画像は `assets/images/` に置きます。

### スライドをpdfでエクスポート

`decktape`を使ってスライドをPDFにエクスポートできます。

1. `decktape`のインストール

```bash
npm install -g decktape
```

2. PDFエクスポート

以下のコマンドで`index.html`で書いたスライドをpdfにエクスポートできます:

```bash
# 16:9のスライドの場合
decktape --size 1920x1080 index.html slides.pdf

# 4:3のスライドの場合
decktape --size 1600x1200 index.html slides.pdf
```

## 免責事項

- 本スライドの内容に従ったいかなる結果において著者は一切の責任を負いません

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

This project uses [reveal.js](https://github.com/hakimel/reveal.js) which is also licensed under the MIT License.
