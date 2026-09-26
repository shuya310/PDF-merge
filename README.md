# Offline PDF Merge / オフラインでPDF結合

**Merge PDFs entirely inside your browser. Your files never leave your computer.**
**PDFの結合を、ブラウザの中だけで。ファイルは一切外に出ません。**

[![Try it now](https://img.shields.io/badge/Try%20it%20now-%E4%BB%8A%E3%81%99%E3%81%90%E4%BD%BF%E3%81%86-24478f)](https://shuya310.github.io/PDF-merge/pdf-merge.html)
[![Latest release](https://img.shields.io/github/v/release/shuya310/PDF-merge)](https://github.com/shuya310/PDF-merge/releases/latest)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

[English](#english) | [日本語](#日本語)

---

## English

Most "free online PDF merge" sites upload your documents to someone else's server.
This tool doesn't. It is **one HTML file**, and all processing happens locally in your browser.

### Why use this?

- 🔒 **Safe for confidential documents.** Contracts, medical records, HR files, and internal documents are never sent anywhere. The page contains no network code at all.
- ✈️ **Works fully offline.** Runs in air-gapped environments, on a plane, or on a closed corporate network. Once you have the file, no internet connection is needed.
- 🌐 **Works in any modern browser.** Chrome, Edge, Firefox, Safari. Nothing to install and no admin rights needed.
- 📄 **Just one file.** Copy `pdf-merge.html` to a USB stick or a shared folder and anyone can use it.
- 🖱️ **Easy to use.** Drag and drop PDFs, drag rows to reorder, then click Merge.
- ⚡ **Fast & lightweight.** Powered by `pdf-lib` for quick merging right in your browser.
- 🌓 **Dark mode.** Follows your system setting automatically.
- 🇬🇧🇯🇵 **English / Japanese UI.** Picks your browser language automatically. Switch anytime with the button in the top right.

### Get started

- **Try it online:** <https://shuya310.github.io/PDF-merge/pdf-merge.html> (it still runs 100% in your browser, and your files are not uploaded)
- **Use it offline:** download `pdf-merge.html` from the [latest release](https://github.com/shuya310/PDF-merge/releases/latest), then double-click it.

### How to use

1. Add PDFs with the button, or drag and drop them anywhere on the window. Files that are not PDFs are ignored.
2. Set the order (they are merged from top to bottom). Click and drag a row, or use the `↑` `↓` buttons.
3. Enter an output file name and click **Merge & Save**.

### Notes

- Encrypted PDFs may not open. Those rows turn red and are skipped.
- Bookmarks are not carried over. Forms and annotations usually are.
- Safari: if saving does not work when you open the file directly, double-click `start.command` (macOS). It serves the page from `127.0.0.1` only.
- The tool is designed for PCs. On phones and tablets, drag rows by the `⋮⋮` handle.

If this tool is useful to you, please give it a ⭐. It helps other people find it.

---

## 日本語

「無料のオンラインPDF結合サイト」の多くは、ファイルを外部のサーバーへアップロードします。
このツールはアップロードしません。**HTMLファイル1つ**だけでできていて、処理はすべてあなたのブラウザの中で完結します。

### ここが便利

- 🔒 **秘匿性の高いファイルも安心。** 契約書・個人情報・社外秘資料も、どこにも送信されません。ページには通信を行う処理が一切含まれていません。
- ✈️ **完全オフラインで動く。** インターネットにつながらない環境（閉域網・機内・オフライン端末）でも使えます。
- 🌐 **いろいろなブラウザで使える。** Chrome / Edge / Firefox / Safari。インストールも管理者権限もいりません。
- 📄 **ファイル1つだけ。** `pdf-merge.html` を USB メモリや共有フォルダに置けば、誰でもすぐ使えます。
- 🖱️ **かんたん操作。** ドラッグ&ドロップで追加し、行をつかんで並べ替えて、ボタンを押すだけです。
- ⚡ **軽くて速い。** `pdf-lib` を使い、ブラウザの中ですばやく結合します。
- 🌓 **ダークモード対応。** OSの設定に合わせて自動で切り替わります。
- 🇯🇵🇬🇧 **日本語 / 英語の画面。** ブラウザの言語に合わせて自動で切り替わります。右上のボタンでいつでも変えられます。

### はじめかた

- **すぐ試す：** <https://shuya310.github.io/PDF-merge/pdf-merge.html> （Web版でも処理はすべてブラウザ内で行われ、ファイルは送信されません）
- **オフラインで使う：** [最新リリース](https://github.com/shuya310/PDF-merge/releases/latest)から `pdf-merge.html` をダウンロードし、ダブルクリックで開きます。

### 使い方

1. ファイルを追加する。ボタンで選ぶか、Finder からウインドウへドラッグ&ドロップ（どこに落としてもOK。PDF以外は無視されます）
2. 順番を入れ替える（上から順に結合されます）
   - 行を**クリックしたまま動かす**（左の `⋮⋮` をつかんでもOK）
   - `↑` `↓` ボタンでも1つずつ動かせる
3. 出力ファイル名を入れて「結合して保存」

Safari で保存がうまくいかない場合は `start.command` をダブルクリックし、開いたページを使ってください（自分のPC内 `127.0.0.1` だけで動きます。終了は Control+C）。

### 仕様メモ

- 暗号化されたPDFは開けない場合があり、その行は赤く表示され結合対象から外れます。
- しおり（ブックマーク）は引き継がれません。フォーム・注釈は多くの場合引き継がれます。
- 出力ファイル名は、PDF内部のタイトル情報にも同じ名前が書き込まれます。
- 今のところPCでの使用を想定しています。スマホ・タブレットでは、行の長押しが画面スクロールに取られることがあります。その場合は `⋮⋮` をつかんでください。

役に立ったら ⭐ をお願いします。ほかの人がこのツールを見つけやすくなります。

---

## Files / ファイル

| Path | Role |
| --- | --- |
| `pdf-merge.html` | The whole app in one file: styles, UI, and script. pdf-lib 1.17.1 is embedded at the end. / これ1つで動く本体。末尾に pdf-lib 1.17.1 を埋め込み済み |
| `index.html` | Redirects to `pdf-merge.html` (for GitHub Pages) / サイトのトップから本体へ転送 |
| `LICENSE` | MIT License |
| `start.command` | Optional local launcher for macOS, mainly for Safari / ローカルサーバーで開くランチャー（任意） |

Reordering works directly on the `items` array: `reorderTo` rewrites the array and `render` redraws the list.
並べ替えは `items` 配列の並びそのものです（`reorderTo` が配列を書き換え、`render` が描き直す）。

## License / ライセンス

[MIT License](LICENSE). Free to use, copy, modify, and share, including for commercial use. Just keep the copyright notice.
自由に使用・複製・改変・再配布できます（商用利用も可）。著作権表示だけ残してください。

Built with [pdf-lib](https://github.com/Hopding/pdf-lib) (MIT).
