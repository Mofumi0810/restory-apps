# Re:Story Apps

呼吸アプリ・声のジャーナル（PWA対応）

## 公開手順（GitHub Pages）

1. GitHubで公開リポジトリを作成（例: `restory-apps`）
2. このフォルダの中身を全部アップロード（フォルダ構造そのまま・ルート直下に）
3. リポジトリの Settings → Pages → Branch: `main` / フォルダ: `/ (root)` → Save
4. 数分後に公開URLが発行される:
   - 入口: `https://<ユーザー名>.github.io/restory-apps/`
   - 呼吸: `.../breath.html`
   - ジャーナル: `.../journal.html`

## 配布時の案内文（読者向け）

> リンクを開いて、ブラウザのメニューから「ホーム画面に追加」を押すと、
> アプリとしてホーム画面に置けます（青いアイコンが目印です）。

## 更新方法

HTMLを差し替えてpushするだけ。Service Workerはネット優先なので、
再訪問時に自動で新版に切り替わります。

## ファイル構成

- `index.html` — 入口ページ（2アプリへのリンク）
- `breath.html` — 呼吸アプリ
- `journal.html` — 声のジャーナル（Obsidian連携）
- `manifest-*.webmanifest` — PWA設定（アプリ名・アイコン）
- `sw.js` — オフラインキャッシュ
- `icon-*.png` — アイコン各サイズ
