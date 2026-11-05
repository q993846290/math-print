# 算数プリント作成

小学1年〜中学3年の計算・図形問題のプリント（問題用紙・解答用紙）を PDF で作るサイトです。
サーバーを使わず、ブラウザの中で Python（Pyodide）を動かして PDF を作ります。GitHub Pages で無料公開できます。

- `index.html` 画面
- `py/bundle.b64.txt` 問題を作るプログラム（worksheets）と reportlab、IPAゴシックを zip にして base64 にしたもの
- `pyodide/` ブラウザで Python を動かすための Pyodide 0.26.4
- `pdf.min.js` / `pdf.worker.min.js` プレビュー表示用の PDF.js 3.11.174

フォントは IPA フォントライセンスの IPAゴシックです。
