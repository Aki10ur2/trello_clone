# trello_clone

このリポジトリは、  
[この Qiita の記事](https://qiita.com/baby-degu/items/f905c8ee972cf46ce11b)で紹介されている Trello のクローンアプリを作成し、  
React.js / Redux の学習を目的としています。

Issues をノート代わりに使用します。

### 実行環境

- Windows10 Home
- Visual Studio Code
- WSL
  - Ubuntu18.04.3 LTS

### 環境構築

```bash

# yarn を install
$ npm i -g yarn 

 # reactに必要なパッケージがビルドインされたモジュール プロジェクト作成が楽ちんになる。
$ yarn global add create-react-app

# PATHが通ってないので通す。
# https://yarnpkg.com/lang/ja/docs/cli/global/
# yarn global bin コマンドは、インストールした実行可能ファイルへのシンボリックリンクを Yarn が格納する場所を表示します。(引用)

# ~/.bash_profileに追記
# export PATH="$PATH:`yarn global bin`"

# 追記した内容を読み込む
$ source ~/.bash_profile 

# WSLの環境だと、react-scriptsがバグる。
# そのため、package.jsonのreact-scriptsのバージョンを3.3.0から3.2.0に戻して再インストール。
$ yarn install

# 作る。
$ create-react-app app

# Reduxを使って勉強してねって書いてあるので入れる。
$ yarn add react-redux

```