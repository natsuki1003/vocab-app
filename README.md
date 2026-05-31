# Vocabulary Deck Player - Stage 5

## 今回の変更

忘却曲線を意識したAnki風スケジューラーを強化しました。

### 追加されたカード状態

- new: 未学習
- learning: 学習中
- review: 復習中
- relearning: 間違えた後の再学習

### ボタンの動き

- 難しい: learning/relearningに入り、セッション内で数枚後に再表示されます
- 普通: 学習中なら次のステップへ進み、復習中なら間隔を伸ばします
- 簡単: reviewに入り、普通より長めの間隔になります
- すごく簡単: さらに長めの間隔になります

### 保存される情報

localStorageに以下を保存します。

- state
- stepIndex
- intervalDays
- easeFactor
- dueAt
- reviews
- lapses
- lastRating

## 注意

これはAnki完全互換ではなく、Anki風の簡易スケジューラーです。
