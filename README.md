# OfficialRailsTutorial_SampleApp

# 覚えておくこと

## generate修正の方法

generate と対になる形で destory と呼ばれるコマンドが存在する、使い方はgenerateと同じ。
これで誤って作成してしまったcontroller+関連ファイルを削除することができる。
modelも同様。

## 動的ページ

yield、layoutを利用することで動的ページ作成を実現することができる。
なお、 3章では値の注入としてprovideを利用した。

## 自動テスト

Guardと呼ばれるgemを使用すると、ファイルの変更を検知して自動でテストを行ってくれる。
なお、設定は Guard File と呼ばれるファイルに書き込む

Guard初期化
> bundle exec guard init

Guard実行
> bundle exec guard

## ハッシュ省略形

ハッシュがメソッド呼び出しの最後の引数である場合は、波括弧を省略できる。

