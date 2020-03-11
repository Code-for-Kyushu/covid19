# 九州 新型コロナウイルス感染症対策サイト

![](https://github.com/Code-for-Kyushu/covid19/workflows/production%20deploy/badge.svg)


[![九州 新型コロナウイルス感染症対策サイト](https://raw.githubusercontent.com/Code-for-Kyushu/covid19/development/static/ogp.png)](https://dev-covid19-kyusyu.netlify.com/)



### 日本語 | English | 

## 貢献の仕方
Issues にあるいろいろな修正にご協力いただけると嬉しいです。

詳しくは[貢献の仕方](./.github/CONTRIBUTING.md)を御覧ください。


## 行動原則
詳しくは[サイト構築にあたっての行動原則](./.github/CODE_OF_CONDUCT.md)を御覧ください。

## ライセンス
本ソフトウェアは、[MITライセンス](./LICENSE.txt)の元提供されています。

## 本家東京サイトから派生したもの

### 【北海道版】新型コロナウイルス感染症対策サイト
[サイトへのリンク](https://stopcovid19.hokkaido.dev/)

[GitHubへのリンク](https://github.com/codeforsapporo/covid19)

## 開発者向け情報

[東京都 新型コロナ対策サイト 地域展開 情報共有 - HackMD](https://hackmd.io/@homata/ryHz3P4BI)


## 開発の始め方

↓にうまくまとまっています。ちょっとだけ違います。
[東京都 新型コロナウイルス対策サイトへの貢献方法を解説 - Qiita](https://qiita.com/FPC_COMMUNITY/items/b9cc072813dc2231b2b2)

まずは自分のリポジトリへ[Code for KyushuのGithubリポジトリ](https://github.com/Code-for-Kyushu/covid19)からフォークしてください。




### 環境構築の手順

- 必要となるNode.jsのバージョン: 10.19.0以上

**yarn を使う場合**
``` bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev
```

**docker compose を使う場合**
```bash
# serve with hot reload at localhost:3000
$ docker-compose up --build
```

### `Cannot find module ****` と怒られた時

**yarn を使う場合**
```
$ yarn install
```

**docker compose を使う場合**
```bash
$ docker-compose run --rm app yarn install
```

### ステージング・本番環境・開発環境へのデプロイ（反映）


`development` ブランチがアップデートされると、自動的に `dev-pages` ブランチにHTML類がbuildされます。そして、開発用サイト https://dev-covid19-kyusyu.netlify.com/ が更新されます。


以下は準備中です

>`master` ブランチがアップデートされると、自動的に `production` ブランチにHTML類がbuildされます。そして、本番サイト https://stopcovid19.metro.kyusyu.lg.jp/ が更新されます。

>`staging` ブランチがアップデートされると、自動的に `gh-pages` ブランチにHTML類がbuildされます。そして、ステージングサイト https://stg-covid19-kyusyu.netlify.com/ が更新されます。

