# 卓球 試合分析ツール（iPhone Safari対応版）

## iPhoneで使う方法
このアプリは、iPhone Safariで**Webサーバーから開く**ことを前提にしています。
`file://` でHTMLを直接開く方式はiOS Safariでは安定しないため、以下のどちらかで公開してください。

### 方法A：GitHub Pages
1. GitHubで新しいリポジトリを作る。
2. このフォルダの `index.html` / `manifest.webmanifest` / `sw.js` をアップロード。
3. GitHub Pagesを有効化。
4. 発行された `https://...` をiPhone Safariで開く。
5. Safariの「共有」→「ホーム画面に追加」でアプリのように起動可能。

### 方法B：その他の静的Webホスティング
3ファイルを同じディレクトリに置いて、HTTPS URLで公開してください。

## 動画について
動画は `<input type=file>` からiPhone上で選択し、ブラウザのObject URLとして再生します。
動画ファイルをアプリのサーバーへアップロードする処理はありません。

## 注意
iPhone Safariで動作させるには、`index.html`を「ファイル」アプリから直接開くのではなく、
HTTPSのWebページとして開いてください。
