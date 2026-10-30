# STC Associate PWA

## 公開方法
このフォルダ内のファイル一式を、HTTPS対応のWebサーバーに同じ構成でアップロードしてください。
`index.html` だけでなく、`manifest.json`、`service-worker.js`、`icons/` も必要です。

## iPhoneへのインストール
1. HTTPSで公開したURLをiPhoneのSafariで開く
2. 共有ボタンをタップ
3. 「ホーム画面に追加」を選択
4. 追加後、ホーム画面の「STC Associate」アイコンから起動

## 注意
- PWAのインストールとService WorkerにはHTTPSが必要です（localhostを除く）。
- Tailwind CSS、Lucide、Chart.js、Google Fontsは外部CDNを利用しています。初回表示時はインターネット接続が必要です。Service Workerは取得済みの外部リソースを可能な範囲でキャッシュしますが、完全なオフライン動作を保証するものではありません。
- 学習履歴はブラウザのlocalStorageに保存されます。ホーム画面アプリとSafariで保存領域が別になる場合があります。
