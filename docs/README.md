{% import "./parts/guide.html" as guide %}

# このサイトについて

ブログやサポートサイトなどに使える「できるだけ簡単な記事公開の仕組み」が欲しいと思いHonKitを使ってみました。セットアップや詰まったことなどをサポートサイトっぽくまとめています。
<br><br>

{{- guide.render("HonKit Documentation", "https://honkit.netlify.app", "https://honkit.netlify.app") }}


## できあがった記事公開の手順

### ![](https://icongr.am/octicons/fold-down.svg?size=32&color=currentColor) クローン

```shell
git clone {repository}
npm ci
```

リポジトリをクローンしてパッケージをインストールします。

これだけでセットアップは完了です。

### ![](https://icongr.am/feather/edit-2.svg?size=32&color=currentColor) 編集

```shell
npm run honkit:serve
```

記事をマークダウンで追加・編集します。

### ![](https://icongr.am/octicons/package.svg?size=32&color=currentColor) ビルド

```shell
npm run honkit:build
```

デプロイ用のファイルを作成します。


### ![](https://icongr.am/octicons/fold-up.svg?size=32&color=currentColor) プッシュ

```shell
git push origin {repository}
```

編集した内容はGitHubに保存します。

### ![](https://icongr.am/feather/github.svg?size=32&color=currentColor) あとはGitHubにおまかせ

```shell
...
```

GitHub Actionを使って自動的にホスティングサービスにデプロイします。

## メリット

- 👍 開発者がいつでも気軽にセットアップできます
- 👍 マークダウンで記事が書けます
- 👍 変更のログがGitHubに残ります
