---
layout: default
title: Nyani Privacy Policy
---

# Nyani Privacy Policy

Last updated: 2026-10-15

[日本語はこちら](#日本語)

Nyani is a set of two-player board games with cats. It has no account and no sign-in, it shows no ads, and it does not track you. This page explains, item by item, what stays on your iPhone, what leaves it, and how long anything is kept.

Nyani is published by Daiki Takatsuki. Contact: the feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5 (choose Nyani as the app).

## The short version

- Your cat, your name and title, and your settings are stored on your iPhone only.
- On one phone, and against the neighbor cats (the computer), the only thing Nyani does online is ask the App Store whether you own Nyani Plus.
- Rooms (two phones) pass game messages through our small relay server so the two phones can reach each other. **Your name is never sent in a room.** The other player sees your title and your cat.
- The relay may keep short-lived technical records, described below. We use them only to run the service and stop abuse.
- Nyani Plus is sold by Apple. Nyani only learns whether you own it.
- There is no analytics SDK, no crash-reporting SDK, no advertising and no tracking.

## What stays on your iPhone

- The cat you chose, the name and title you set, and your sound setting.
- Whether you own Nyani Plus (a copy of what the App Store tells the app).
- The series score of the games you play in a row is kept in memory only, never saved. It is cleared when you leave the match or the room, or close the app.

Deleting the app deletes all of this.

## Rooms (playing on two phones)

To connect two phones, Nyani uses a relay server we run on Cloudflare Workers.

What passes through it while you are in a room:

- The 6-digit room number, and the room key inside the QR code or link.
- Your title and the kind of cat you chose, so the other player can see them. Your name is not sent.
- The game the host picked, each move, and the stamps you send (stamps are fixed pictures with fixed words; there is no free-text chat).
- Whether the host owns Nyani Plus, so the other player can play the Plus games in that room.
- The version numbers of the room messages and of each game's rules, so two different app versions don't start a game that would go out of step.

What the relay keeps:

- For each room: the room number, its state, when it was created, and hashed (not readable) seat tokens and room key. Moves and stamps are passed on and not stored.
- A room nobody connects to is deleted about 10 minutes after it was created. Otherwise it is deleted within about 30 minutes after the last person disconnects.
- Your IP address is used for 1 minute to limit how often rooms can be created or joined.
- Cloudflare, which hosts the relay, may record technical logs of requests (such as the time, the address requested and the IP address). Any such logs are kept for no more than 30 days and are used only to keep the service running and to stop abuse. See [Cloudflare's privacy policy](https://www.cloudflare.com/privacypolicy/).

None of this is linked to your identity, used for advertising, or shared with anyone else.

## Camera

The camera is used only to scan a room's QR code. Nothing is recorded or sent.

## Photos

When you share a result card and choose Save Image, iOS asks for permission to add a photo. Nyani can only add the image you chose to save. It never reads your photos.

## Sharing a result card

The result card image is made on your iPhone. It shows the cats, the score and the winner (on one phone, the winner's name; in a room, the title). It goes only to the app you pick in the share sheet.

## Nyani Plus (in-app purchase)

Purchases are handled by Apple. Nyani never sees your payment details. It only learns from Apple whether you own Nyani Plus.

## No third parties in the app

Nyani contains no analytics, advertising, crash-reporting or tracking code.

## If you contact us

The feedback form is a Google Form. It does not ask for your name or email address. If you open it from Settings in Nyani, the app's name and version and your iOS version are already filled in, so we can tell which app and version a report is about. You can see and change them before you send. What you write is stored in Google Forms and used only to fix problems and improve the app. We delete it when it is no longer needed for that. To ask us to delete something you sent, send the form again and describe the message. See [Google's privacy policy](https://policies.google.com/privacy).

## What Apple tells us

Apple gives developers aggregated reports, such as downloads, and crash reports from people who chose to share them with developers in their iPhone settings. These do not identify you to us.

## Your choices

You can play without rooms, and then nothing about your games leaves your iPhone. Deleting the app removes everything stored on it.

## Children

Nyani does not ask anyone, including children, for personal information.

## Changes to this policy

If this policy changes, we will update this page and the date at the top.

## Contact

The feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5 (choose Nyani as the app).

---

## 日本語

最終更新日: 2026-10-15

Nyani は猫と遊ぶ 2 人用のボードゲーム集です。アカウントもサインインもなく、広告もトラッキングもありません。何が iPhone の中に残り、何が外へ出て、どのくらいの期間残るのかを、項目ごとに書きます。

Nyani の提供者は Daiki Takatsuki です。連絡先: フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5 （アプリは Nyani を選んでください）

### 要約

- 選んだ猫、名前と二つ名、設定は、iPhone の中にだけ置きます。
- 1 台で遊ぶとき、近所の猫（コンピューター）と遊ぶときに Nyani が通信するのは、App Store に Nyani Plus を持っているかを確かめるときだけです。
- 部屋（2 台で遊ぶ）では、2 台がつながるために、私たちの小さな中継サーバーを通して対局の文を受け渡します。**部屋で名前を送ることはありません。** 相手に見えるのは、二つ名と猫です。
- 中継には、下に書く短い期間の技術的な記録が残ることがあります。使うのは、サービスを動かすことと、悪用を止めることだけです。
- Nyani Plus を販売するのは Apple です。Nyani が知るのは、持っているかどうかだけです。
- 分析・クラッシュ報告・広告・トラッキングのための SDK は入っていません。

### iPhone の中に置くもの

- 選んだ猫、決めた名前と二つ名、効果音の設定。
- Nyani Plus を持っているか（App Store がアプリに伝えた内容の写し）。
- 続けて遊んだ局の連戦スコアは、メモリの中だけに持ち、保存しません。対局や部屋を抜けるか、アプリを閉じると消えます。

アプリを削除すると、これらはすべて消えます。

### 部屋（2 台で遊ぶ）

2 台をつなぐために、私たちが Cloudflare Workers で動かしている中継サーバーを使います。

部屋にいるあいだに通るもの:

- 6 桁の部屋の番号と、QR コードやリンクに入っている部屋の鍵。
- 相手に見せるための、二つ名と選んだ猫の種類。名前は送りません。
- 部屋主が選んだゲーム、1 手ずつの手、送ったスタンプ（スタンプは決まった絵と決まった言葉だけで、自由に書くチャットはありません）。
- 部屋主が Nyani Plus を持っているか（その部屋で相手も Plus のゲームを遊べるようにするため）。
- 部屋の文の形の版と、ゲームの決まりの版（版の違う 2 台で対局がずれないようにするため）。

中継が持つもの:

- 部屋ごとに、部屋の番号・状態・作った時刻と、席の札と部屋の鍵のハッシュ（元に戻せない形）。手とスタンプは受け渡すだけで、保存しません。
- 誰もつながらなかった部屋は、作ってから約 10 分で消えます。それ以外の部屋は、最後の人が切れてから約 30 分以内に消えます。
- IP アドレスは、部屋を作る・入る回数を制限するために 1 分間だけ使います。
- 中継を動かしている Cloudflare は、リクエストの技術的な記録（時刻・宛先・IP アドレスなど）を残すことがあります。残す場合も 30 日以内とし、サービスを動かすことと悪用を止めることにだけ使います。[Cloudflare のプライバシーポリシー](https://www.cloudflare.com/ja-jp/privacypolicy/) もご覧ください。

これらをあなたが誰かと結びつけたり、広告に使ったり、ほかの人に渡したりすることはありません。

### カメラ

カメラは部屋の QR コードを読むときだけ使います。記録も送信もしません。

### 写真

結果の札を共有して「画像を保存」を選ぶと、iOS が写真に追加してよいかを聞きます。Nyani ができるのは、選んだ画像を写真に足すことだけです。写真を読むことはありません。

### 結果の札を送る

結果の札の画像は iPhone の中で作ります。猫・スコア・勝った人（1 台では名前、部屋では二つ名）が入ります。共有シートで選んだアプリにだけ渡ります。

### Nyani Plus（App 内課金）

購入の処理は Apple が行います。Nyani が支払いの情報を見ることはありません。Apple から、Nyani Plus を持っているかどうかだけを受け取ります。

### アプリの中の第三者

分析・広告・クラッシュ報告・トラッキングのためのコードは入っていません。

### お問い合わせいただいたとき

フォームは Google フォームです。名前もメールアドレスも聞きません。Nyani の設定から開くと、どのアプリのどの版についてのご連絡かが分かるよう、アプリの名前と版・iOS の版が入った状態で開きます。送る前に確かめて、書き換えられます。書いていただいた内容は Google フォームに保存され、不具合の修正とアプリの改善にだけ使い、要らなくなったら消します。送った内容を消してほしいときは、もう一度フォームから、どの内容かを書いて送ってください。[Google のプライバシーポリシー](https://policies.google.com/privacy?hl=ja) もご覧ください。

### Apple から届くもの

Apple は開発者に、ダウンロード数などの集計と、iPhone の設定で開発者との共有を選んだ人のクラッシュの記録を渡します。私たちがそこからあなたを特定することはできません。

### 選べること

部屋を使わずに遊べば、対局について iPhone の外へ出るものはありません。アプリを削除すると、iPhone に置いたものはすべて消えます。

### お子さまについて

Nyani は、お子さまを含め、誰にも個人情報を求めません。

### このポリシーの変更

変えるときは、このページと冒頭の日付を更新します。

### 連絡先

フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5 （アプリは Nyani を選んでください）
