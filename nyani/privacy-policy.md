---
layout: default
title: Nyani Privacy Policy
---

# Nyani Privacy Policy

Last updated: 2026-10-14

[日本語はこちら](#日本語)

Nyani is a set of two-player board games with cats. It has no account and no sign-in, and it does not collect data about you: not for analytics, not for advertising, not in anonymized form. This page explains, item by item, what stays on your iPhone and what leaves it.

Nyani is published by Daiki Takatsuki. Contact: the feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5

## The short version

- Your cat, your name and title, and your settings are stored on your iPhone only. The series score is kept in memory only.
- Playing on one phone or against the neighbor cats (the computer) uses no network at all.
- Rooms (two phones) pass messages through our small relay server so the two phones can reach each other. The relay does not store your moves or your name.
- Nyani Plus is sold by Apple. Nyani only learns whether you own it.
- There is no analytics SDK, no crash-reporting SDK, no advertising and no tracking.

## What stays on your iPhone

- The cat you chose, the name and title you set, and your sound setting.
- The series score of the games you play in a row is kept in memory only, never saved. It is gone when you leave the match or close the app.
- Whether you own Nyani Plus (a copy of what the App Store tells the app).

Deleting the app deletes all of this.

## Rooms (playing on two phones)

To connect two phones, Nyani uses a relay server we run on Cloudflare Workers (room-relay.cookiso862.workers.dev).

What passes through it while you are in a room:

- The 6-digit room number, and the room key inside the QR code or link.
- Your name, your title and the kind of cat you chose, so the other player can see them.
- The game the host picked, each move, and the stamps you send.
- Whether the host owns Nyani Plus, so the other player can play the Plus games in that room.

What the relay keeps: only that the room exists, its state, and hashed (not readable) seat tokens and room key. It does not write your moves, name or cat to storage, and its request logs are turned off. A waiting room is deleted after 10 minutes, and a room is deleted when everyone has left.

Like any internet service, Cloudflare receives your IP address when your phone connects. We do not keep it.

## Camera

The camera is used only to scan a room's QR code. Nothing is recorded or sent.

## Photos

When you share a result card and choose Save Image, iOS asks for permission to add a photo. Nyani can only add the image you chose to save. It never reads your photos.

## Sharing a result card

The result card image is made on your iPhone. It goes only to the app you pick in the share sheet.

## Nyani Plus (in-app purchase)

Purchases are handled by Apple. Nyani never sees your payment details. It only learns from Apple whether you own Nyani Plus.

## No third parties in the app

Nyani contains no analytics, advertising, crash-reporting or tracking code.

## What Apple tells us

Apple gives developers aggregated reports, such as downloads, and crash reports from people who chose to share them with developers in their iPhone settings. These do not identify you to us.

## Children

Nyani does not collect personal information from anyone, including children.

## Changes to this policy

If this policy changes, we will update this page and the date at the top.

## If you contact us

The feedback form is a Google Form. It does not ask for your name or email address. What you write is stored in Google Forms and used only to fix problems and improve the app.

## Contact

The feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5 (choose Nyani as the app).

---

## 日本語

最終更新日: 2026-10-14

Nyani は猫と遊ぶ 2 人用のボードゲーム集です。アカウントもサインインもなく、あなたについてのデータを集めません（分析にも、広告にも、匿名化した形でも）。何が iPhone の中に残り、何が外へ出るかを、項目ごとに書きます。

Nyani の提供者は Daiki Takatsuki です。連絡先: フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5

### 要約

- 選んだ猫、名前と二つ名、設定は、iPhone の中にだけ置きます。連戦スコアはメモリの中だけに持ちます。
- 1 台で遊ぶとき、近所の猫（コンピューター）と遊ぶときは、通信を一切しません。
- 部屋（2 台で遊ぶ）では、2 台がつながるために、私たちの小さな中継サーバーを通して文を受け渡します。中継は手も名前も保存しません。
- Nyani Plus を販売するのは Apple です。Nyani が知るのは、持っているかどうかだけです。
- 分析・クラッシュ報告・広告・トラッキングのための SDK は入っていません。

### iPhone の中に置くもの

- 選んだ猫、決めた名前と二つ名、効果音の設定。
- 続けて遊んだ局の連戦スコアは、メモリの中だけに持ち、保存しません。対局を抜けるか、アプリを閉じると消えます。
- Nyani Plus を持っているか（App Store がアプリに伝えた内容の写し）。

アプリを削除すると、これらはすべて消えます。

### 部屋（2 台で遊ぶ）

2 台をつなぐために、私たちが Cloudflare Workers で動かしている中継サーバー（room-relay.cookiso862.workers.dev）を使います。

部屋にいるあいだに通るもの:

- 6 桁の部屋の番号と、QR コードやリンクに入っている部屋の鍵。
- 相手に見せるための、あなたの名前・二つ名・選んだ猫の種類。
- 部屋主が選んだゲーム、1 手ずつの手、送ったスタンプ。
- 部屋主が Nyani Plus を持っているか（その部屋で相手も Plus のゲームを遊べるようにするため）。

中継が持つのは、部屋があること・部屋の状態・席の札と部屋の鍵のハッシュ（元に戻せない形）だけです。手・名前・猫は保存先に書かず、アクセスの記録も切ってあります。待っている部屋は 10 分で消え、全員が抜けた部屋も消えます。

ほかのインターネットのサービスと同じく、つなぐときに Cloudflare は IP アドレスを受け取ります。私たちはそれを残しません。

### カメラ

カメラは部屋の QR コードを読むときだけ使います。記録も送信もしません。

### 写真

結果の札を共有して「画像を保存」を選ぶと、iOS が写真に追加してよいかを聞きます。Nyani ができるのは、選んだ画像を写真に足すことだけです。写真を読むことはありません。

### 結果の札を送る

結果の札の画像は iPhone の中で作ります。共有シートで選んだアプリにだけ渡ります。

### Nyani Plus（App 内課金）

購入の処理は Apple が行います。Nyani が支払いの情報を見ることはありません。Apple から、Nyani Plus を持っているかどうかだけを受け取ります。

### アプリの中の第三者

分析・広告・クラッシュ報告・トラッキングのためのコードは入っていません。

### Apple から届くもの

Apple は開発者に、ダウンロード数などの集計と、iPhone の設定で開発者との共有を選んだ人のクラッシュの記録を渡します。私たちがそこからあなたを特定することはできません。

### お子さまについて

Nyani は、お子さまを含め、誰からも個人情報を集めません。

### このポリシーの変更

変えるときは、このページと冒頭の日付を更新します。

### お問い合わせいただいたとき

フォームは Google フォームです。名前もメールアドレスも聞きません。書いていただいた内容は Google フォームに保存され、不具合の修正とアプリの改善にだけ使います。

### 連絡先

フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5（アプリは Nyani を選んでください）
