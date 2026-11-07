# プリント作成

小学1年〜中学3年の算数・数学プリント（問題用紙・解答用紙）を PDF で作るサイトです。
サーバーを使わず、ブラウザの中で Python（Pyodide）を動かして PDF を作ります。GitHub Pages で無料公開できます。

## できること

- 計算・文章題・図形・関数（グラフ）・データなど約110単元から、出題範囲と問題数を選ぶ
- 複数日分を1つの PDF にまとめる。日にちごとに単元・問題数を選び直すこともできる
- 大問構成（単元ごとに「1 次の計算をしなさい。」のようにまとめる）
- 書体は教科書風（日本語は IPAex明朝、数式は KaTeX の書体）

## ファイル

- `index.html` 画面
- `py/bundle.b64.txt` 問題を作るプログラム（worksheets）と reportlab を zip にして base64 にしたもの
- `fonts/` IPAex明朝（IPAフォントライセンス）、KaTeX フォント（MIT ライセンス）
- `pyodide/` ブラウザで Python を動かすための Pyodide 0.26.4
- `pdf.min.js` / `pdf.worker.min.js` プレビュー表示用の PDF.js 3.11.174
