# Vocabulary Deck Player - Stage 2

## 今回の目的

Anki風のWebアプリ化に向けて、複数の単語帳をCSVで管理できる形にしています。

今回の重要ポイントは、単語帳ごとに違うCSVヘッダーを使えるようにしたことです。

## ファイル構成

vocab-app/
  index.html
  decks.json
  decks/
    ielts-task1-map.csv
    ielts-task2-academic.csv
    daily-conversation.csv

## 仕組み

- `decks.json` に単語帳一覧を書く
- 各単語帳は `file` で読み込むCSVを指定する
- 各単語帳は `schema` で「CSVのどの列をカードのどの項目として使うか」を指定する

## メイン単語帳

今作り込む想定のメイン単語帳はこれです。

decks/ielts-task1-map.csv

このCSVは以下の日本語ヘッダーを使っています。

番号,単語,品詞,発音記号,意味,短い意味,ニュアンス解説,コロケーション,例文_英語,例文_日本語,言い換え,メモ

## 他の仮デッキ

他の2つは将来拡張用の仮デッキです。

- ielts-task2-academic.csv: 英語ヘッダー
- daily-conversation.csv: 最小限ヘッダー

違うヘッダーでも、`decks.json` の `schema` を書けば表示できます。

## GitHubへのアップロード方法

ZIPを解凍して、中身をGitHubリポジトリの一番上にアップロードしてください。

重要: ZIPファイルそのものではなく、中身をアップロードしてください。
