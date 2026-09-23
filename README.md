# Offline PDF Merge Tool

A simple and secure web-based tool to combine multiple PDF files into one. All processing is done locally in your browser — **no files are uploaded to any server, ensuring complete privacy.**

> ⭐️ **If you find this project useful, please consider giving it a star!**

---

### Key Features
- 🔒 **100% Offline & Private:** Your sensitive documents never leave your browser.
- ⚡ **Fast & Lightweight:** Powered by `pdf-lib` for quick client-side merging.
- 🖱️ **Drag & Drop:** Easily reorder PDFs using intuitive drag-and-drop or simple up/down controls.
- 🌓 **Dark Mode Support:** Clean user interface with automatic dark mode support.

---

### How to Use
1. Download or clone this repository.
2. Double-click `pdf-merge.html` to open it in your web browser.
   *(For Safari users: If you experience issues saving files, double-click `start.command` to run a local server, then open the page.)*
3. Drag & drop your PDF files into the window or click the button to select them.
4. Drag rows (hold for ~0.2s) or use the arrow buttons to rearrange the page order.
5. Enter your desired output filename and click **"Merge & Save"**.

---

### Limitations & Notes
- **Encrypted PDFs:** Password-protected or encrypted PDFs cannot be opened. These will be highlighted in red and excluded from the output.
- **Bookmarks:** PDF bookmarks are not preserved. Forms and annotations are mostly retained.
- **Title Metadata:** The output filename will also be set as the internal title metadata of the generated PDF.
---
# オフラインでPDF結合システム 

複数のPDFを順番を決めて1つのPDFに結合するツール。処理は全てブラウザの中で完結し、**外部への通信は一切ありません。**

※今のところPCでの使用のみです

## 使い方

`pdf-merge.html` をダブルクリックしてブラウザで開く。
（Safari で保存がうまくいかない場合は `start.command` をダブルクリックし、開いたページを使う。終了は Control+C）

1. ファイルを追加する。ボタンで選ぶか、Finder からウインドウへドラッグ&ドロップ（どこに落としてもOK。PDF以外は無視されます）
2. 順番を入れ替える（上から順に結合されます）
   - 行を**長押し（約0.2秒）してそのまま動かす**か、左の `⋮⋮` をつかんで動かす
   - `↑` `↓` ボタンでも1つずつ動かせる
3. 出力ファイル名を入れて「結合して保存」

## ファイル

| パス | 役割 |
| --- | --- |
| `pdf-merge.html` | 画面の構造と処理（約330行） |
| `pdf-merge.css` | 見た目（ダークモード対応込み） |
| `lib/pdf-lib.min.js` | PDF操作ライブラリ pdf-lib 1.17.1 |
| `start.command` | ローカルサーバーで開くランチャー（任意）※主にSafari |

## 仕様メモ

- 暗号化されたPDFは開けない場合があり、その行は赤く表示され結合対象から外れます。
- しおり（ブックマーク）は引き継がれません。フォーム・注釈は多くの場合引き継がれます。
- 出力ファイル名は、PDF内部のタイトル情報にも同じ名前が書き込まれます。
- 並べ替えは `items` 配列の並びそのものです（`reorderTo` が配列を書き換え、`render` が描き直す）。
- スマホ・タブレットでは、行の長押しは画面スクロールに取られることがあります。その場合は `⋮⋮` をつかんでください。
