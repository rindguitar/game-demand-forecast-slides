# game-demand-forecast-slides

## 概要

[game-demand-forecast](https://github.com/rindguitar/game-demand-forecast) の発表用スライドです。

「Steamレビューの感情分析モデルは本当に良くなったのか？」を統計で検証した話を、
以下のIssueの内容に沿って紹介します:

- [#21](https://github.com/rindguitar/game-demand-forecast/issues/21) 既製汎用モデルとのOOD性能比較（ファインチューニング効果の検証）
- [#19](https://github.com/rindguitar/game-demand-forecast/issues/19) 感情分析モデルの高精度化（DAPT）
- [#25](https://github.com/rindguitar/game-demand-forecast/issues/25) 評価が訓練データ固定だった問題の修正
- [#24](https://github.com/rindguitar/game-demand-forecast/issues/24) 多シード検証によるDAPT効果の頑健性

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

## クレジット

本スライドは [reveal.js](https://github.com/hakimel/reveal.js)（MIT License）を利用して作成しています。
