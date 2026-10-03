# AI Game Center Hackathon

## 辞書的定義

AIによる画像・音声の判定を遊びに組み込む、ブラウザゲームの試作集です。ゲームごとに独立した HTML と README があり、共通のサーバーアプリを導入する構成ではありません。

## 用語としての用例

- 「AI Pose Tetris で手の形を次のブロックにする」: カメラ画像を判定してテトリスの操作に取り込みます。
- 「多言語発音チャレンジで日本語の空耳発音を採点する」: マイクで録音し、指定言語らしい音の特徴をAIに評価させるゲームです。

## 思想的背景

各ゲームの説明に共通する狙いは、ポーズや声といった身体的な入力を、AIの判定を介してゲームの反応へつなぐことです。発音スコアはゲーム内の評価であり、語学能力の認定を目的とするものではありません。

## 技術的背景・入口

- [AI Pose Tetris](ai-pose-tetris/README.md): HTML / JavaScript、Canvas、Web Audio API、Geminiによる画像判定。[本体](ai-pose-tetris/index.html)
- [多言語発音チャレンジ](multilingual-pronunciation-challenge/README.md): HTML / JavaScript、マイク録音、Web Audio / Web Speech API、Geminiによる音声判定。[本体](multilingual-pronunciation-challenge/index.html)
- [画面資料](assets/README.md): assets 配下の資料案内。

## 歴史的背景

リポジトリ名には 20260816 を含みますが、それだけから開催日・参加実績は断定しません。確認できる履歴として、[2026年9月5日の更新](https://github.com/masa-san-jp/20260816-ai-game-center-hackathion/commit/c1eaf879d79dabdb790002aeeb036636feb7b956) と、各ゲームのコード・説明が保存されています。

## 展開・利用上の注意

試すゲームの README で操作と実行方法を確認してください。画像・録音はAI APIへ送信する構成のため、カメラ・マイクの許可と送信範囲を確認し、映り込みや第三者の音声を含めないでください。モデル・API設定、利用枠、ブラウザの権限に依存する試作であり、この資料整備ではAPI接続や公開運用を検証していません。
