# Vocabulary Deck Player - Stage 1

## この段階でできること

- デッキ一覧画面を表示する
- `decks.json` からデッキ情報を読み込む
- `decks/` フォルダ内のCSVを読み込む
- CSVの単語をカードとして表示する
- 単語と例文をブラウザ音声で再生する

## GitHubにアップロードする構成

vocab-app/
  index.html
  decks.json
  decks/
    ielts-task1-map.csv
    ielts-task2-academic.csv
    daily-conversation.csv

## 単語を追加する方法

1. 対象のCSVをスプレッドシートで編集する
2. CSVとして保存する
3. GitHub上の同じCSVファイルを上書きする
4. Commit changes を押す
5. GitHub Pagesのページを開いて強制更新する

## CSVヘッダー

番号,単語,品詞,発音記号,意味,短い意味,ニュアンス解説,コロケーション,例文_英語,例文_日本語,言い換え,メモ
