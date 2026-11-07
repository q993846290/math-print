# プリント作成

小学1年〜中学3年の算数・数学プリント（問題用紙・解答用紙）を PDF で作るサイトです。
サーバーを使わず、ブラウザの中で Python（Pyodide）を動かして PDF を作ります。GitHub Pages で無料公開できます。

## できること

- 計算・文章題・図形・関数（グラフ）・データなど約110単元から、出題範囲と問題数を選ぶ
- 複数日分を1つの PDF にまとめる。日にちごとに単元・問題数を選び直すこともできる
- 大問構成（単元ごとに「1 次の計算をしなさい。」のようにまとめる）
- 書体は、日本語が丸ゴシック（Zen Maru Gothic）、数字・数式が TeX 風（KaTeX の書体）

## ファイル

- `index.html` 画面
- `py/bundle-*.b64.txt` 問題を作るプログラム（worksheets）と reportlab を zip にして base64 にしたもの
- `fonts/` Zen Maru Gothic（SIL Open Font License 1.1）、KaTeX フォント（MIT ライセンス）
- `pyodide/` ブラウザで Python を動かすための Pyodide 0.26.4
- `pdf.min.js` / `pdf.worker.min.js` プレビュー表示用の PDF.js 3.11.174
