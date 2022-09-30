{% import "./parts/guide.html" as guide %}

<nav class="breadcrumbs">
  <span>トップ</span>
</nav>

# このサイトについて

架空アプリのサポートサイトです。

初期構築なしで手軽に記事を投稿できるサイトを作っています。

## 記事の投稿手順

### ![](https://icongr.am/octicons/fold-down.svg?size=32&color=currentColor) クローン

```sh
git clone {repository}
```

### ![](https://icongr.am/feather/edit-2.svg?size=32&color=currentColor) 編集

```sh
npm run honkit:serve
```

### ![](https://icongr.am/octicons/fold-up.svg?size=32&color=currentColor) プッシュ

```sh
git push origin {repository}
```

### ![](https://icongr.am/feather/github.svg?size=32&color=currentColor) あとはGitHubにおまかせ

```sh
...
```

## もっと知りたい

<div class="grid grid-cols-2 gap-8">
  {{- guide.render("はじめてガイド", "#", "初心者さん向けガイドです。") }}
  {{- guide.render("リリースノート", "#", "機能アップデートのお知らせです。") }}
</div>
