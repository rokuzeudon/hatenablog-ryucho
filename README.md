# Ryucho

Ryucho は、はてなブログ用テーマです。

[Hatena-Blog-Theme-Boilerplate](https://github.com/hatena/Hatena-Blog-Theme-Boilerplate/releases)をベースにしています。

# セットアップ

SCSSで開発する場合は、下記の手順でリポジトリのcloneとモジュールのインストールを行います。

## Required Component

- [Node.js](https://nodejs.org/)

## モジュールのインストール

```
$ git clone git@github.com:hatena/Hatena-Blog-Theme-Boilerplate.git
$ cd Hatena-Blog-Theme-Boilerplate
$ npm install
```

# 通常のテーマ開発

下記のコマンドで、SCSSファイル変更の監視とコンパイルを行います。

```
$ npm start
```

また、コンパイル後 `build/boilerplate.css` が作られます。

つづいて、[はてなブログ](https://blog.hatena.ne.jp/)の設定を行います。

1. テーマ検証に使うブログを1つ用意します。
1. 1.で作成したブログの「デザイン設定」にアクセスし、「カスタマイズ」タブの「デザインCSS」の内容を下記に置き換えて保存します。

```
@import url("http://localhost:3000/boilerplate.css");
```

※ Browsersync のブラウザ自動リロードはサポートしていません。

## （オプション）レスポンシブデザインのテーマ開発

レスポンシブデザインのテーマを開発する場合、ブログの「デザイン設定」->「カスタマイズ」にアクセスし、「デザインCSS」欄の先頭に下記のコメントを挿入してください。

```
/* Responsive: yes */
```

ヘルプ: [レスポンシブデザインのテーマを作成する際の注意点 - はてなブログ ヘルプ](http://help.hatenablog.com/entry/theme/custom-theme#responsive)

