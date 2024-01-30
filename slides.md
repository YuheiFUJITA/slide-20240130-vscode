---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shikiji
lineNumbers: false
info: |
  [VS Code Meetup \#27 \- connpass](https://vscode.connpass.com/event/303633/)で登壇したスライドです。

  アーカイブは[YouTube](https://www.youtube.com/watch?v=2YH3mhkkJcw)にあります。
drawings:
  persist: false
transition: slide-left
title: 闇鍋VS Codeをプロファイル機能できれいにする | VS Code Meetup \#27
mdc: true
---

# 闇鍋VS Codeを<br>プロファイル機能で<br>きれいにする

2024-01-30@VS Code Meetup

Yuhei FUJITA

---

# 自己紹介

<div class="grid grid-cols-4 gap-4">

<div>


![icon](https://github.com/YuheiFUJITA.png)

</div>
<div class="col-span-3">

- 名前: Yuhei FUJITA（<ruby>藤<rt>ふじ</rt></ruby><ruby>田<rt>た</rt></ruby> <ruby>悠<rt>ゆう</rt></ruby><ruby>平<rt>へい</rt></ruby>）
- X(Twitter): [@Yuhei_FUJITA](https://twitter.com/Yuhei_FUJITA)
- GitHub: [@YuheiFUJITA](https://github.com/YuheiFUJITA)
- コミュニティ運営: [Vue Fes](https://vuefes.jp/) / [PWA Night](https://pwanight.connpass.com/) / [VS Code Meetup](https://vscode.connpass.com/)
- 趣味: [キャンプ](https://x.com/Yuhei_FUJITA/status/1748854045664829587) / [フィルムカメラ](https://www.instagram.com/yuhei_fujita.film/)

</div>
</div>

---
layout: statement
---

# VS Codeの闇鍋化

---

# 生まれたてのVS Code

まだ汚れを知らない、とても美しい姿をしている

![生まれたてのVS Code](/images/vscode-bady.png)

---

# 闇鍋化したVS Code

きっと幾億もの開発を経験してきたんだろう、面構えが違う

![闇鍋化した](/images/vscode-rip.png)

---

# 闇鍋VS Codeとは

- 無数の拡張機能がインストールされている
  - フロントエンド用、サーバーサイド用、データベース用、etc...
  - 実際使うのはそのうちの一部のみ
- 無数の設定が入り乱れている
  - 拡張機能が増えれば自ずと設定も増える
  - よく見るともう無効な設定まで残ってる
- おっっっもい
  - 起動するだけで時間がかかる
  - コーディングしててもなんかもっさりする

---
layout: statement
---

# プロファイル機能で救おう

---

# プロファイル機能とは

- VS Codeのあれやこれやをプロファイル単位で管理できる機能
  - Chromeのプロファイル機能みたいなもの
- 任意のワークスペースで任意のプロファイルを利用可能
  - git管理するものではないので他の共同開発者には影響しない
- ユーザー設定や拡張機能などを一括で切り替えられる
  - フロントエンド用、サーバーサイド用などを用意しておくと便利

---

# プロファイルで切り替えられるもの

- 設定
  - `settings.json` の中身
- キーボードショートカット
  - `keybindings.json` の中身
- スニペット
  - 設定しているスニペット
- UIの状態
  - `globalState.json` の中身
- 拡張機能
  - インストールしている拡張機能リスト

---

# プロファイルの新規作成

<div class="grid grid-cols-5 gap-4">
<div class="col-span-2">

![Alt text](/images/profile-create.gif)

</div>
<div class="col-span-3">

1. **メニュー > プロファイル > <br>プロファイルの作成...** を選択
2. プロファイル名・コピー元・アイコン・<br>構成内容を指定
3. 作成する
4. 作成したプロファイルに切り替わる

</div>
</div>

---

# プロファイルの切り替え

<div class="grid grid-cols-5 gap-4">
<div class="col-span-2">

![Alt text](/images/profile-switch.gif)

</div>
<div class="col-span-3">

1. **メニュー > プロファイル > <br>切り替えたいプロファイル名** を選択
2. 選択したプロファイルに切り替わる

</div>
</div>

---

# プロファイルのエクスポート

<div class="grid grid-cols-5 gap-4">

<div class="col-span-2">

![Alt text](/images/profile-export.gif)

</div>
<div class="col-span-3">

1. 事前にエクスポートしたいプロファイルに<br>切り替えておく
2. **メニュー > プロファイル > <br>プロファイルをエクスポート...** を選択
3. 出力先を選択する
4. JSONフォーマットとして出力される

gistに直接エクスポートすることも可能

</div>
</div>

---

# プロファイルのインポート

<div class="grid grid-cols-5 gap-4">
<div class="col-span-2">

![Alt text](/images/profile-import.gif)

</div>
<div class="col-span-3">

1. **メニュー > プロファイル > <br>プロファイルをインポート...** を選択
2. インポート元を選択する
3. インポートしたプロファイルに切り替わる

gistのURLからインポートすることも可能

</div>
</div>

---

# まとめ

- 1つのプロファイルにすべてを詰め込むとVS Codeが闇鍋化する
- プロファイル機能を使うことでVS Codeを用途ごとの最小構成にできる
- 言語やフレームワークごとなどでプロファイルを用意しておくと便利

---

# 関連情報

- [Visual Studio Code January 2023](https://code.visualstudio.com/updates/v1_75#_profiles)
- [Profiles in Visual Studio Code](https://code.visualstudio.com/docs/editor/profiles)
