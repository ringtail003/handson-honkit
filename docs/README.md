{% import "./parts/guide.html" as guide %}

# このサイトについて

ブログやサポートサイトなどに使える「できるだけ簡単な記事公開の仕組み」が欲しいと思い [HonKit](https://honkit.netlify.app/setup.html) を使ってみました。セットアップや詰まったことなどをサポートサイトっぽくまとめています。
<br><br>
このサイト自身もHonKitで作っています。

## できあがった記事公開の手順

### ![](https://icongr.am/octicons/fold-down.svg?size=32&color=currentColor) クローン

```sh
git clone {repository}
```

### ![](https://icongr.am/feather/edit-2.svg?size=32&color=currentColor) 編集

```sh
npm run honkit:serve
```

### ![](https://icongr.am/octicons/package.svg?size=32&color=currentColor) ビルド

```sh
npm run honkit:build
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
