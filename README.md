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

# 5章

## ファイルアクセス高速化

Railsはassets直下にディレクトリを分けて構成している、このおかげでブラウザ側からはassets直下に全てのファイルが存在する認識となり、
フラットなディレクトリとして認識される。このおかげでアクセス高速化される。

## アセットパイプライン
ファイル群を最小化してくれる。

* アセットディレクトリ
    各環境下で静的ファイルを目的別に分類する。
* マニフェストファイル
    各静的ファイル群をどのように1つにまとめるか書かれている。
* プリプロセッサエンジン
    ブラウザに配信できるようにそれらをマニフェストファイルを用いて結合し、サイトテンプレート用に準備する。