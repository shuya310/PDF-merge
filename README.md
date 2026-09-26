# Offline PDF Merge / オフラインでPDF結合

**Merge PDFs entirely inside your browser. Your files never leave your computer.**
**PDFの結合を、ブラウザの中だけで。ファイルは一切外に出ません。**

[![Try it now](https://img.shields.io/badge/Try%20it%20now-%E4%BB%8A%E3%81%99%E3%81%90%E4%BD%BF%E3%81%86-24478f)](https://shuya310.github.io/PDF-merge/pdf-merge.html)
[![Latest release](https://img.shields.io/github/v/release/shuya310/PDF-merge)](https://github.com/shuya310/PDF-merge/releases/latest)
![No upload](https://img.shields.io/badge/upload-none-2e7d32)
![Single HTML file](https://img.shields.io/badge/single-HTML%20file-555)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

[English](#english) | [日本語](#日本語)

---

## English

Let's be honest: most "free online PDF merge" sites quietly upload your documents to someone else's server.
This one doesn't. It's just **one HTML file**, and everything happens locally, right there in your browser.

### Why you'll like it

- 🔒 **Great for stuff you don't want floating around.** Contracts, medical records, HR files — none of it goes anywhere. There's no network code in the page at all.
- ✈️ **Works completely offline.** Air-gapped machine, plane wifi, locked-down corporate network — doesn't matter. Once you've got the file, you're good.
- 🌐 **Runs in whatever browser you've got.** Chrome, Edge, Firefox, Safari. No install, no admin rights, nothing.
- 📄 **Just one file.** Drop `pdf-merge.html` on a USB stick or a shared folder and anyone can use it.
- 🖱️ **Dead simple.** Drag and drop your PDFs, drag rows to reorder, hit Merge.
- ⚡ **Fast.** `pdf-lib` does the heavy lifting, right there in the browser.
- 🌓 **Dark mode**, following your system setting automatically.
- 🇬🇧🇯🇵 **English / Japanese UI.** Picks your browser's language automatically, and you can flip it anytime with the button top-right.

### Get started

- **Try it online:** <https://shuya310.github.io/PDF-merge/pdf-merge.html> (still 100% browser-side, nothing gets uploaded)
- **Use it offline:** grab `pdf-merge.html` from the [latest release](https://github.com/shuya310/PDF-merge/releases/latest) and double-click it.

### How to use it

1. Add your PDFs — click the button or drag them onto the window. Anything that's not a PDF gets ignored.
2. Put them in order (top to bottom = merge order). Drag a row, or use the `↑` `↓` buttons.
3. Type a file name, hit **Merge & Save**. Done.

### Good to know

- Encrypted PDFs might not open — those rows turn red and get skipped automatically.
- Bookmarks don't carry over. Forms and annotations usually do.
- Built with PCs in mind. On phones/tablets, grab the `⋮⋮` handle to drag rows around.

If this saved you some time, a ⭐ would be awesome — it helps other people find it too.

---

## 日本語

「無料のオンラインPDF結合」系のサイトって、だいたいファイルをどこかのサーバーに送ってるんですよね。
このツールはそれをしません。**HTMLファイル1つ**だけでできていて、処理は全部あなたのブラウザの中で完結します。

### ここが便利

- 🔒 **秘匿性の高いファイルでも安心。** 契約書・個人情報・社外秘資料も、どこにも送信されません。ページに通信処理は一切入っていません。
- ✈️ **完全オフラインで動く。** 閉域網でも機内でも、ネットが無くても大丈夫。ファイルさえあればOKです。
- 🌐 **好きなブラウザで使える。** Chrome / Edge / Firefox / Safari、インストールも管理者権限も不要です。
- 📄 **ファイルはたった1つ。** `pdf-merge.html` をUSBメモリや共有フォルダに置いておけば、誰でもすぐ使えます。
- 🖱️ **操作はシンプル。** ドラッグ&ドロップで追加、行をつかんで並べ替えて、ボタンを押すだけ。
- ⚡ **軽くてサクサク。** `pdf-lib` がブラウザの中でサッと結合してくれます。
- 🌓 **ダークモード対応。** OSの設定に合わせて自動で切り替わります。
- 🇯🇵🇬🇧 **日本語 / 英語の画面。** ブラウザの言語で自動判定、右上のボタンでいつでも切り替えられます。

### はじめかた

- **すぐ試す：** <https://shuya310.github.io/PDF-merge/pdf-merge.html>（Web版でも処理は全部ブラウザ内。ファイルは送信されません）
- **オフラインで使う：** [最新リリース](https://github.com/shuya310/PDF-merge/releases/latest)から `pdf-merge.html` をダウンロードして、ダブルクリック。

### 使い方

1. ファイルを追加する。ボタンで選ぶか、Finderからウインドウへドラッグ&ドロップ（どこに落としてもOK、PDF以外は無視されます）
2. 順番を入れ替える（上から順に結合されます）
   - 行をつかんで動かす（左の `⋮⋮` でもOK）
   - `↑` `↓` ボタンで1つずつ動かしてもOK
3. 出力ファイル名を入れて「結合して保存」を押すだけ

### 仕様メモ

- 暗号化されたPDFは開けないことがあります。その行は赤く表示されて、結合対象から自動で外れます。
- しおり（ブックマーク）は引き継がれません。フォーム・注釈はだいたい引き継がれます。
- 出力ファイル名は、PDF内部のタイトル情報にも同じ名前が書き込まれます。
- PCでの使用を想定しています。スマホ・タブレットでは `⋮⋮` をつかんで並べ替えてください。

役に立ったら ⭐ をもらえると嬉しいです。ほかの人がこのツールを見つけやすくなります。

---

## Files / ファイル

| Path | Role |
| --- | --- |
| `pdf-merge.html` | The whole app in one file: styles, UI, and script. pdf-lib 1.17.1 is embedded at the end. / これ1つで完結する本体。末尾に pdf-lib 1.17.1 を埋め込み済み |
| `LICENSE` | MIT License |

Reordering just works on the `items` array directly — `reorderTo` rewrites it, `render` redraws the list.
並べ替えは `items` 配列そのものを操作しています（`reorderTo` が並びを書き換えて、`render` が描き直すだけ）。

## License / ライセンス

[MIT License](LICENSE). Use it, copy it, tweak it, ship it — commercial use included. Just keep the copyright notice.
自由に使用・複製・改変・再配布できます（商用利用もOK）。著作権表示だけ残してください。

Built with [pdf-lib](https://github.com/Hopding/pdf-lib) (MIT).
