# Website

This website is built using [Docusaurus 2](https://docusaurus.io/), a modern static website generator.

### Installation

```
$ yarn
```

### Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
$ yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

### Deployment

Using SSH:

```
$ USE_SSH=true yarn deploy
```

Not using SSH:

```
$ GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.

## ページの追加方法

いくつか方法がある。

* `src/pages` 配下に追加する方法
* `blog` 配下に追加する方法 
* `docs` 配下に追加する方法 

|ディレクトリ|説明|
|-|-|
|src/pages|通常の Web サイトのようなページを作成する場合はこちらに作成する。主にルートページ（/）を配置するときに使う。React や Markdown、mdx を活用して追加ができる。<br>https://docusaurus-i18n-staging.netlify.app/ja/docs/creating-pages|
|docs|ドキュメントを配置することを目的にしたディレクトリ。デフォルトだと URL は /docs 配下となるが、 / に変更もできる。Markdown、mdx に対応。<br>https://docusaurus-i18n-staging.netlify.app/ja/docs/docs-introduction|
|blog|ブログの投稿を目的にしたディレクトリ。Markdown、mdx に対応。<br>https://docusaurus.io/docs/blog|
|static|主に画像はこちらに格納する。| 
