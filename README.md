# Rails Factory

Railsのprojectを簡単に作成する。

## 必要なもの
- Ruby (latest version): Railsでサポートしているversion
    - rbenv (latest version)
    - ruby build (latest version)
- Bundler (latest version)

## 作り方
1. Gemfileで使いたいRailsのversionを記載する
    - 5.2.3の場合: `gem "rails", "5.2.3"`
        - rbenvで5.2.3がサポートしているRubyに切り替える
1. bundle install
    - Globalを汚染しない様にGemを `/vendor/bundle` 直下にインストールする様に設定。
1. `bundle exec rails --version` でRailsのインストールを確認。
1. `bundle exec rails new [projectName] -d mysql -T -B` でproject作成
    - 作りたいprojectによってoptionは変更。
1. 他のところへ持っていって開発開始👍

## 参考
- どこかの記事を参考にしたけど思い出せない…
