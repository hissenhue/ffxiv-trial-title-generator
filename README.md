# FF14 Trial Title Generator

Final Fantasy XIV風の討滅戦タイトル画面を簡単に作成できるWebアプリケーションです。

## 特徴

- **FF14風デザイン**: 本家のゲームに近いタイトル画面デザイン
- **カスタマイズ可能**: サブタイトル、英語タイトル、日本語タイトルを自由に設定
- **背景画像対応**: カスタム背景画像のアップロード機能
- **高品質出力**: SVGベースで1920x1080の高解像度PNG出力
- **ソーシャル対応**: Twitter/X、Facebook、LINEでのリッチプレビュー対応

## 使い方

1. ブラウザで `index.html` を開く
2. テキストフィールドに好きな文字を入力
3. 必要に応じて背景画像をアップロード
4. 「タイトル画面を生成」ボタンでプレビュー更新
5. 「画像を保存」ボタンでPNG形式でダウンロード

## 技術仕様

- **フロントエンド**: HTML5 + CSS3 + Vanilla JavaScript
- **グラフィック**: SVG + Canvas API
- **フォント**: Google Fonts (Cinzel + Noto Serif JP)
- **出力形式**: PNG (1920x1080px)
- **ブラウザ対応**: モダンブラウザ全般

## ファイル構成

```
├── index.html           # メインアプリケーション
├── back-image.jpg       # デフォルト背景画像
├── ogp-image.jpg        # ソーシャルメディア用プレビュー画像
├── README.md           # このファイル
├── LICENSE             # MITライセンス
└── CLAUDE.md           # 開発者向けガイド
```

## ライセンス

MIT License - 詳細は [LICENSE](LICENSE) ファイルを参照してください。