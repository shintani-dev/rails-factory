# Rails Factory

Rails の project を簡単に作成する。

## 必要なもの

- Ruby (latest version): Rails でサポートしている version
  - rbenv (latest version)
  - ruby build (latest version)
- Bundler (latest version)

## 使い方

1. `Gemfile` で使いたい Rails の version を記載する
   - 6.0.3.2 の場合: `gem "rails", "6.0.3.2"`
1. rbenv で 6.0.3.2 がサポートしている Ruby に切り替える
   - 2.7.1
1. `vender` ディレクトリがある場合は削除する
   - `$ rm -rf vernder`
1. ↑ で指定した Rails をインストールする
   - `$ bundle install`
1. Rails のインストールを確認
   - `$ bundle exec rails -v`
1. project 作成
   - `$ bundle exec rails new project/[projectName] -d mysql -T -B`
   1. 作りたい project によって option は変更
      - `$ bundle exec rails -h` で詳細確認可能
      - 以下、主要な option
        - `-d` : データベース
          - mysql/postgresql/sqlite3
        - `-T` : テストは導入しない
          - 作るプロジェクトで選択可能とする
        - `-B` : `bundle install` を行わない
          - 作るプロジェクトで必要な Gem を選択可能とする
1. 他のところへ持っていって開発開始 👍

## ライセンス

[MIT ライセンス](LICENSE)

## 参考

- どこかの記事を参考にしたけど思い出せない…
