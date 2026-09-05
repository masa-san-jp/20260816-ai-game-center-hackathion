# 🖐️ AI Hand Tetris (AIハンド・テトリス)

カメラの前で作った**「手の形（ジオメトリ）」**をAIがリアルタイム解析し、それに応じたテトリスブロック（I, J, L, O, S, T, Z）を落としてプレイする新感覚のウェブゲームです。

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Gemini AI](https://img.shields.io/badge/Gemini_3_Flash-8E7CC3?style=flat-square&logo=googlecloud&logoColor=white)

---

## 🌟 特徴

1. **手の形（ジオメトリ）でブロック決定**
   - 画面の前でグーや手のひら、L字などの形を作るだけで、AI（Google Gemini API）が形状を幾何学的に測定し、最も近いテトリスブロックを生成します。
2. **高速・軽量レスポンス**
   - 撮影画像を軽量化・最適化処理してAI送信するため、3秒のカウントダウン撮影後に**爆速で判定**が完了します。
3. **1画面完結のレスポンシブデザイン**
   - カメラ映像・スコアボード・ゲーム画面・操作ガイドがスクロールなしで1画面（ワンビュー）に美しく収まります。
4. **インストール不要**
   - ブラウザとカメラがあれば、PCでもスマホでもすぐに遊べます。

---

## 🎮 遊び方 & 手の形ガイド

### 基本ルール
1. **START GAME** ボタンを押してゲームを開始します。
2. ブロックが落下・固定されるたびに、画面上で**3秒間の撮影カウントダウン**（3 → 2 → 1）がスタートします。
3. カウント0の瞬間にカメラの前で**「特定の形」**を作って静止してください。
4. AIが判定したブロックが「NEXT（次の落下ブロック）」として画面に登場します。

### 手の形とブロックの対応表

| ブロック | 手の形 (Hand Geometry) | 特徴・作り方のコツ |
| :---: | :--- | :--- |
| **I 型** | **平らな手** | 指をまっすぐ閉じて、1本の細長い形状を作る |
| **O 型** | **グー（拳）** | 手をしっかり握って、四角くコンパクトな塊を作る |
| **T 型** | **T字交差** | 片方の手のひらを、もう片方の手首に直角（90度）に当てる |
| **L / J 型** | **L字ハンド** | 親指と人差し指で90度の「L」の形を作る（鏡像でJ型） |
| **S / Z 型** | **クランク手** | 手のひらや指をジグザグ（クランク状）に曲げる |

---

## ⌨️ 操作方法

キーボードまたは画面下のタッチボタンでブロックを操作します。

| 操作 | キーボード | スマホ・画面操作 |
| :--- | :--- | :--- |
| **左右移動** | `←` / `→` キー | 左右矢印ボタン |
| **ソフトドロップ** | `↓` キー | 下矢印ボタン |
| **ハードドロップ** | `↑` キー | DROP ボタン |
| **左回転** | `Z` キー | ↺ (Z) ボタン |
| **右回転** | `C` キー | ↻ (C) ボタン |

---

## 📁 ファイル構成

ai-hand-tetris/
├── index.html              # メインのHTML・ゲームロジック・UI
└── README.md               # プロジェクト説明書（本書）

---

## 🛠️ 技術スタック

- **フロントエンド**: HTML5, Canvas API, JavaScript (ES6+), Tailwind CSS
- **アイコン / フォント**: Font Awesome 6, Google Fonts (Orbitron / Noto Sans JP)
- **AI 判定モデル**: Google Gemini API (`gemini-3-flash-preview`)
- **オーディオ**: Web Audio API (SE効果音自動生成)

---

## 🚀 ローカルでの実行方法

1. 本リポジトリのコードをダウンロードします。
2. `index.html` をブラウザ（Google Chrome / Safari / Edge等）で開きます。
3. カメラの使用許可ダイアログが表示されたら「許可」を選択してください。

---

## 📄 ライセンス

MIT License
