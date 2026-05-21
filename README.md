# Vocabulary Deck Player - Stage 3

## 今回の変更

### 1. Startボタンによる自動カード送りを廃止
前の版では Start を押すと、自動で音声再生しながら次の単語へ進みました。
今回からこれは廃止しました。

### 2. Auto Audioボタンを追加
Auto Audio: On のとき:
- カードが表示されたら単語と例文を自動再生します。

Auto Audio: Off のとき:
- 自動再生しません。
- 再生ボタンまたは Replay を押した時だけ音声再生します。

### 3. Anki風の4つの復習ボタンを追加
- 難しい: 5分後
- 普通: 1日後
- 簡単: 2日後
- すごく簡単: 3日後

ボタンを押すと、そのカードの復習予定日がブラウザに保存され、次の復習対象カードへ進みます。

### 4. 学習履歴をlocalStorageに保存
ブラウザを閉じても、同じブラウザで開けば復習予定が残ります。

注意:
- PCのChromeとスマホのSafariでは履歴は共有されません。
- 番号または単語を変えると、別カードとして扱われる場合があります。
- 今回は簡易スケジューラーです。Anki完全互換ではありません。

## ファイル構成

vocab-app/
  index.html
  decks.json
  decks/
    ielts-task1-map.csv
    ielts-task2-academic.csv
    daily-conversation.csv
