# XSA - X Search Assistant

[![Deploy to GitHub Pages](https://github.com/msonrm/XSA/actions/workflows/deploy.yml/badge.svg)](https://github.com/msonrm/XSA/actions/workflows/deploy.yml)
[![PWA](https://img.shields.io/badge/PWA-enabled-blue.svg)](https://web.dev/progressive-web-apps/)

複数キーワードを効率的にX(Twitter)検索できるPWA（Progressive Web App）です。

## 🚀 主な機能

- **複数キーワード検索**: 複数のキーワードを一度にOR検索
- **除外キーワード**: 不要なキーワードを除外して検索精度を向上
- **検索セット保存**: よく使う検索パターンをローカルに保存
- **共有機能**: QRコードやURLで検索セットを簡単共有
- **PWA対応**: オフラインでも動作、ホーム画面に追加可能
- **レスポンシブデザイン**: モバイル・デスクトップ対応

## 🛠 技術スタック

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **PWA機能**: Service Worker, Web App Manifest
- **UI/UX**: iOS風デザインシステム
- **データ圧縮**: LZ-string
- **QRコード**: qrcode-generator
- **ホスティング**: GitHub Pages

## 📱 使い方

### 基本的な使い方

1. **検索セット名**を入力（例：「推し海外文学作家」）
2. **検索キーワード**を改行区切りで入力
   ```
   ミルハウザー
   カルヴィーノ
   ピンチョン
   プルースト
   ```
3. **除外キーワード**があれば入力（省略可能）
4. 「🔍 検索してみる」でXの検索結果を確認

### 便利機能

- **💾 検索セットを保存**: よく使うセットをローカル保存
- **📤 共有リンクを生成**: QRコードやURLで他の人と共有
- **📱 ホーム画面に追加**: PWAとしてインストール可能

## 🔧 セットアップ

### GitHub Pages デプロイ

1. このリポジトリをフォークまたはクローン
2. GitHub リポジトリの Settings > Pages でソースを設定
3. `https://yourusername.github.io/XSA/` でアクセス可能

### ローカル開発

```bash
# リポジトリをクローン
git clone https://github.com/msonrm/XSA.git
cd XSA

# ローカルサーバーを起動（例: Python）
python -m http.server 8000
# または
python3 -m http.server 8000

# ブラウザで http://localhost:8000 にアクセス
```

## 📁 ファイル構成

```
XSA/
├── index.html          # メインのHTMLファイル
├── manifest.json       # PWAマニフェスト
├── sw.js              # Service Worker
├── icon-192.png       # PWAアイコン (192x192)
├── icon-512.png       # PWAアイコン (512x512)
├── screenshot-mobile.png   # モバイル版スクリーンショット
├── screenshot-desktop.png  # デスクトップ版スクリーンショット
├── 404.html           # GitHub Pages用エラーページ
├── .gitignore         # Git除外設定
└── README.md          # このファイル
```

## 🌟 主な特徴

### PWA機能
- **オフライン対応**: Service Workerによるキャッシュ
- **インストール可能**: ホーム画面への追加
- **レスポンシブ**: モバイル・タブレット・デスクトップ対応

### UX/UI
- **iOS風デザイン**: 直感的で洗練されたインターフェース
- **ダークモード対応**: システム設定に自動追従
- **アニメーション**: 滑らかなトランジション効果

### データ管理
- **ローカルストレージ**: 検索セットをブラウザに保存
- **圧縮共有**: LZ-stringによる効率的なURL共有
- **QRコード**: 簡単な共有とインポート

## 🤝 コントリビューション

Issue や Pull Request をお待ちしています！

### 開発ガイドライン

1. 新機能は feature ブランチで開発
2. コミットメッセージは日本語で分かりやすく
3. PWA のベストプラクティスに従う
4. モバイルファーストでレスポンシブ対応

## 📄 ライセンス

MIT License - 詳細は [LICENSE](LICENSE) ファイルを参照

## 🔗 関連リンク

- [Web App Manifest](https://web.dev/add-manifest/)
- [Service Worker](https://web.dev/service-worker/)
- [X(Twitter) Search API](https://developer.twitter.com/en/docs/twitter-api)

---

**Created by [@msonrm](https://github.com/msonrm)**