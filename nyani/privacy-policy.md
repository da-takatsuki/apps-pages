---
layout: default
title: Nyani Privacy Policy
---

# Nyani Privacy Policy

Last updated: 2026-10-24

[日本語はこちら](#日本語)

Nyani is a set of two-player board games with cats. It has no account and no sign-in, it shows no ads, and it does not track you. This page explains, item by item, what stays on your iPhone, what leaves it, and how long anything is kept.

Nyani is published by Daiki Takatsuki. Contact: the feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5 (choose Nyani as the app).

## The short version

- Your cat, your name and title, your game records and your settings are stored on your iPhone.
- Nyani asks the App Store whether you own Nyani Plus, and asks our relay server how your invitations are going (see "Invite friends, get Plus"). On one phone and against the neighbor cats (the computer), these are the only things Nyani does online.
- Rooms (two phones) pass game messages through our small relay server so the two phones can reach each other. **In a room, your name is sent to the other player** after Nyani checks it against the name rules and masks inappropriate words. The relay passes it on and does not store it.
- The relay keeps the short-lived records and the invitation records described below. We use them only to run the service and stop abuse.
- Nyani Plus and the treats are sold by Apple. Nyani only learns what you own.
- There is no analytics SDK, no crash-reporting SDK, no advertising and no tracking.

## What stays on your iPhone

- The cat you chose, the name and title you set, and the collar charm your cat wears.
- Your settings: music, sound effects, vibration and music volume.
- Your game records. For each finished game: when it was played, which game, who you played (the other player's name and cat, or which neighbor cat) and the result. Nyani keeps the latest 5,000 games. The Records screen and the friend shown next to your cat on Home are made from these records. They are not sent anywhere.
- When you last opened the app, so your cat can greet you after a while away.
- Whether you own Nyani Plus and which treats you have given (a copy of what the App Store tells the app).
- Small markers so the same notice is not shown twice (for example, that you have already seen the Plus offer or a thank-you for an invitation).
- A copy of how your invitations are going: the number of friends counted and the offer codes given to you.
- The invite key (see "Invite friends, get Plus"), kept in the iPhone Keychain.

Deleting the app deletes all of this except the invite key, which iOS keeps in the Keychain.

## Rooms (playing on two phones)

To connect two phones, Nyani uses a relay server we run on Cloudflare Workers.

What passes through it while you are in a room:

- The 6-digit room number, and the room key inside the QR code or link.
- Your name, your title, the kind of cat you chose and its collar charm, so the other player can see them. Before your name is sent, Nyani checks it against the name rules (up to 12 characters, no links, no runs of 4 or more digits) and masks inappropriate words. If your name breaks the rules, it is not sent, and the other player sees your title instead. The other player's iPhone checks it again when it arrives.
- The game the host picked, each move, and the stamps you send (stamps are fixed pictures with fixed words; there is no free-text chat).
- Whether the host owns Nyani Plus, so the other player can play the Plus games in that room.
- The version numbers of the room messages and of each game's rules, so two different app versions don't start a game that would go out of step.
- The list of games your version of Nyani has, so the host only picks a game both phones can play.
- When the host creates a room, the host's invite key, so that a friend who joins can be counted for the host. The relay keeps only a one-way hash of it.
- When a friend finishes their first game in a room, a DeviceCheck token from the friend's iPhone (see "Invite friends, get Plus").

What the relay keeps:

- For each room: the room number, its state, when it was created, and hashed (not readable) seat tokens and room key. If the host's app sent an invite key, the room also keeps its hash and the answers to "was this friend counted". Names, moves and stamps are passed on and not stored.
- A room nobody connects to is deleted about 10 minutes after it was created. Otherwise it is deleted within about 30 minutes after the last person disconnects.
- Your IP address is used for 1 minute to limit how often rooms can be created or joined, how often invitations can be checked, how often a friend can be counted, and how often a player can be removed from a room.
- Cloudflare, which hosts the relay, processes request data such as the time, the address requested and your IP address to deliver and protect the service, under [its own privacy policy](https://www.cloudflare.com/privacypolicy/). Any request logs we can access are kept for no more than 30 days and are used only to run the service and stop abuse.

We do not connect any of this to your name, Apple ID, email address or contact details, use it for advertising, or share it with anyone else.

## Invite friends, get Plus

Nyani gives Plus for free when friends join you. Your iPhone makes a random number for invitations (the invite key). It sends the key to the relay server to read your progress when you open the app, when you open your profile, the invite screen or the reward screen, and when a friend is counted in your room. It is also sent when you create a room. It is sent even if you have never invited anyone.

What the relay server stores, once at least one friend has been counted for you (until then, it stores nothing about your invitations):

- A one-way hash of the invite key. The key itself is not stored.
- The number of friends counted.
- The offer codes (for the App Store) given to you, and the dates they expire.
- The times those records were made and updated.

What the relay server does not store:

- Names, titles, cats, moves or boards.
- A friend's device identifier, or Apple's DeviceCheck token. The token is only passed to Apple.
- Contacts, email addresses or location.

How counting works: a friend counts as one when they finish a game in your room, as long as their iPhone has never been counted before and has never finished a game as the host of a room. Each device is counted only once. To avoid counting the same device twice, Nyani uses Apple's DeviceCheck. DeviceCheck keeps two bits per device on Apple's side, and Nyani uses one of them to remember only that this device was counted. Nyani's server holds no identifier of your friend's device. Deleting and reinstalling the app does not make that device count again. Friends are not counted in test builds (TestFlight).

How long it is kept: offer codes in our stock are deleted 30 days after they expire, including the stock entry for a code given to you. Your invitation record (the key's hash, the count, the codes given to you and their expiry dates, and the times made and updated) is not deleted automatically for now, so that past thank-yous can still be shown. The invite key stays in your iPhone's Keychain even after you delete the app, and it does not move to another device. The relay server does not connect your invitation record to a name or an Apple ID.

Redeeming a code happens on Apple's screen, and Apple handles the purchase.

## Camera

The camera is used only to scan a room's QR code. Nothing is recorded or sent.

## Photos

When you share a result card and choose Save Image, iOS asks for permission to add a photo. Nyani can only add the image you chose to save. It never reads your photos.

## Sharing a result card

You can share the result card after any game, including a game in a room. The image is made on your iPhone. It shows both cats, the winner's name, the score and, when there is one, your record against the other player with their name (in a room, the name shown after the name check). It goes only to the app you pick in the share sheet.

## Nyani Plus and treats (in-app purchases)

Purchases are handled by Apple. Nyani never sees your payment details. It only learns from Apple whether you own Nyani Plus and which treats you have given.

## No third parties in the app

Nyani contains no analytics, advertising, crash-reporting or tracking code.

## If you contact us

The feedback form is a Google Form. It does not ask for your name or email address. If you open it from Settings in Nyani, the app's name and version and your iOS version are already filled in, so we can tell which app and version a report is about. You can see and change them before you send. What you write is stored in Google Forms and used only to fix problems and improve the app. We delete it when it is no longer needed for that. To ask us to delete something you sent, send the form again and describe the message. See [Google's privacy policy](https://policies.google.com/privacy).

If you report a player from a room, the form opens with the room number, that player's name (or title, if no name was shown), their cat and the time already filled in, so we can look into it. Your own name is not included. You can see and change it before you send. We use reports only to deal with abuse, and delete them when they are no longer needed for that.

## What Apple tells us

Apple gives developers aggregated reports, such as downloads, and crash reports from people who chose to share them with developers in their iPhone settings. These do not identify you to us.

## Your choices

You can play without rooms. Then nothing about your games leaves your iPhone; only the checks with the App Store and with our relay about your invitations go online. If you don't want your name shown in a room, change it on your profile before you join. Deleting the app removes everything stored on it except the invite key in the Keychain.

## Children

Nyani does not ask anyone, including children, for a real name, email address, phone number or location. The name you enter is a nickname kept on your iPhone; in a room it is shown to the other player after the name check, and the relay does not store it. Apart from the short-lived room records described above, the only ID the relay keeps is the one-way hash of the invite key described in "Invite friends, get Plus".

## Changes to this policy

If this policy changes, we will update this page and the date at the top.

## Contact

The feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5 (choose Nyani as the app).

---

## 日本語

最終更新日: 2026-10-24

Nyani は猫と遊ぶ 2 人用のボードゲーム集です。アカウントもサインインもなく、広告もトラッキングもありません。何が iPhone の中に残り、何が外へ出て、どのくらいの期間残るのかを、項目ごとに書きます。

Nyani の提供者は Daiki Takatsuki です。連絡先: フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5 （アプリは Nyani を選んでください）

### 要約

- 選んだ猫、名前と二つ名、対局の成績、設定は、iPhone の中に置きます。
- Nyani は、App Store に Nyani Plus を持っているかを確かめ、私たちの中継サーバーに招待の進み具合を問い合わせます（「友だちを誘って Plus」を見てください）。1 台で遊ぶとき、近所の猫（コンピューター）と遊ぶときに通信するのは、この 2 つだけです。
- 部屋（2 台で遊ぶ）では、2 台がつながるために、私たちの小さな中継サーバーを通して対局の文を受け渡します。**部屋では、あなたの名前を相手に送ります。** 送る前に名前の決まりに通し、不適切な語は伏せ字にします。中継は受け渡すだけで、保存しません。
- 中継には、下に書く短い期間の記録と、招待の記録が残ります。使うのは、サービスを動かすことと、悪用を止めることだけです。
- Nyani Plus と応援のおやつを販売するのは Apple です。Nyani が知るのは、何を持っているかだけです。
- 分析・クラッシュ報告・広告・トラッキングのための SDK は入っていません。

### iPhone の中に置くもの

- 選んだ猫、決めた名前と二つ名、猫が着けている首輪のチャーム。
- 設定（BGM、効果音、振動、BGM の音量）。
- 対局の成績。終わった 1 局ごとに、遊んだ日時、ゲーム、相手（相手の名前と猫、または近所のどの猫か）、勝敗を残します。残すのは新しいほうから 5,000 局までです。成績の画面と、ホームで猫の隣に出る友だちは、この成績から作ります。どこにも送りません。
- 最後にアプリを開いた時刻（しばらくぶりに開いたとき、猫があいさつするため）。
- Nyani Plus を持っているか、どの応援のおやつを差し入れたか（App Store がアプリに伝えた内容の写し）。
- 同じ知らせを 2 度出さないための小さな印（Plus の案内や、招待のお礼をもう見たか、など）。
- 招待の進み具合の写し（数えた友だちの人数と、あなたに渡されたオファーコード）。
- 招待の鍵（「友だちを誘って Plus」を見てください）。iPhone のキーチェーンに置きます。

アプリを削除すると、キーチェーンにある招待の鍵のほかは、すべて消えます。招待の鍵は iOS がキーチェーンに残します。

### 部屋（2 台で遊ぶ）

2 台をつなぐために、私たちが Cloudflare Workers で動かしている中継サーバーを使います。

部屋にいるあいだに通るもの:

- 6 桁の部屋の番号と、QR コードやリンクに入っている部屋の鍵。
- 相手に見せるための、名前、二つ名、選んだ猫の種類、首輪のチャーム。名前は、送る前に名前の決まり（12 文字まで、リンクを含まない、4 桁以上の数字が並ばない）に通し、不適切な語を伏せ字にします。決まりに外れる名前は送らず、相手には二つ名が見えます。受けた相手の iPhone でも、もう一度同じ決まりに通します。
- 部屋主が選んだゲーム、1 手ずつの手、送ったスタンプ（スタンプは決まった絵と決まった言葉だけで、自由に書くチャットはありません）。
- 部屋主が Nyani Plus を持っているか（その部屋で相手も Plus のゲームを遊べるようにするため）。
- 部屋の文の形の版と、ゲームの決まりの版（版の違う 2 台で対局がずれないようにするため）。
- あなたの版の Nyani で遊べるゲームの一覧（部屋主が、2 台とも遊べるゲームだけを選べるようにするため）。
- 部屋を作るときに送る、部屋主の招待の鍵（入ってきた友だちを部屋主の招待として数えるため）。中継は、元に戻せない形（ハッシュ）にして持ちます。
- 友だちが部屋で初めての 1 局を終えたときに送る、友だちの iPhone の DeviceCheck の token（「友だちを誘って Plus」を見てください）。

中継が持つもの:

- 部屋ごとに、部屋の番号・状態・作った時刻と、席の札と部屋の鍵のハッシュ（元に戻せない形）。部屋主のアプリが招待の鍵を送ったときは、そのハッシュと、友だちを数えたかどうかの答えも持ちます。名前、手、スタンプは受け渡すだけで、保存しません。
- 誰もつながらなかった部屋は、作ってから約 10 分で消えます。それ以外の部屋は、最後の人が切れてから約 30 分以内に消えます。
- IP アドレスは、部屋を作る・入る回数、招待を問い合わせる回数、友だちを数える回数、部屋から相手を退出させる回数を制限するために、1 分間だけ使います。
- 中継を動かしている Cloudflare は、サービスを届けて守るために、時刻・宛先・IP アドレスなどのリクエストの情報を、[Cloudflare 自身のプライバシーポリシー](https://www.cloudflare.com/ja-jp/privacypolicy/) に沿って扱います。私たちが見られるリクエストの記録は 30 日以内とし、サービスを動かすことと悪用を止めることにだけ使います。

これらを、あなたの名前・Apple ID・メールアドレス・連絡先と結びつけたり、広告に使ったり、ほかの人に渡したりすることはありません。

### 友だちを誘って Plus

Nyani には、友だちを誘うと Plus が無料になる仕組みがあります。あなたの iPhone は、招待用の乱数（招待の鍵）を作ります。招待の進み具合を読むため、アプリを開いたとき、プロフィール・招待の画面・お礼の画面を開いたとき、部屋で友だちが数えられたときに、この鍵を中継サーバーへ送ります。部屋を作るときにも送ります。誰も誘ったことがなくても送ります。

友だちが 1 人でも数えられると、中継サーバーに次のものを置きます（それまでは、招待について何も置きません）。

- 招待の鍵を元に戻せない形にした値（ハッシュ）。鍵そのものは置きません。
- 数えた友だちの人数。
- あなたに渡したオファーコード（App Store で使うコード）と、その使える期限。
- 上の記録を作った時刻と、更新した時刻。

中継サーバーに置かないもの:

- 名前、二つ名、猫、手や盤面。
- 友だちの端末の識別子や、Apple の DeviceCheck の token。token は Apple に渡すだけです。
- 連絡先、メールアドレス、位置情報。

数え方: 友だちがあなたの部屋で 1 局を最後まで遊ぶと、1 人と数えます。ただし、その友だちの iPhone が、前に数えられたことがなく、部屋主として 1 局を終えたこともない場合に限ります。同じ端末は 1 回しか数えません。同じ端末を 2 度数えないために、Apple の DeviceCheck を使います。DeviceCheck では、Apple が端末ごとに 2 つの印を持ちます。Nyani はそのうち 1 つを使い、この端末を数えたかどうかだけを覚えます。Nyani のサーバーは、友だちの端末を見分ける識別子を持ちません。アプリを消して入れ直しても、その端末は二度と数えません。テスト用の版（TestFlight）では、友だちを数えません。

消す時期: 在庫のオファーコードは、期限から 30 日たつと消します（あなたに渡したコードの在庫の行も含みます）。招待の記録（鍵のハッシュ、人数、あなたに渡したコードとその期限、作った・更新した時刻）は、前に届いたお礼を画面に出せるよう、今のところ自動では消しません。招待の鍵は、アプリを消しても iPhone のキーチェーンに残り、別の端末には移りません。中継サーバーは、招待の記録を名前や Apple ID と結び付けません。

コードの引き換えは Apple の画面で行い、購入の処理は Apple が行います。

### カメラ

カメラは部屋の QR コードを読むときだけ使います。記録も送信もしません。

### 写真

結果の札を共有して「画像を保存」を選ぶと、iOS が写真に追加してよいかを聞きます。Nyani ができるのは、選んだ画像を写真に足すことだけです。写真を読むことはありません。

### 結果の札を送る

結果の札は、どの局のあとでも共有できます（部屋の局も含みます）。画像は iPhone の中で作り、2 匹の猫・勝った人の名前・スコアと、あれば相手との通算（相手の名前つき。部屋では名前の決まりを通った名前）が入ります。共有シートで選んだアプリにだけ渡ります。

### Nyani Plus と応援のおやつ（App 内課金）

購入の処理は Apple が行います。Nyani が支払いの情報を見ることはありません。Apple から受け取るのは、Nyani Plus を持っているかと、どの応援のおやつを差し入れたかだけです。

### アプリの中の第三者

分析・広告・クラッシュ報告・トラッキングのためのコードは入っていません。

### お問い合わせいただいたとき

フォームは Google フォームです。名前もメールアドレスも聞きません。Nyani の設定から開くと、どのアプリのどの版についてのご連絡かが分かるよう、アプリの名前と版・iOS の版が入った状態で開きます。送る前に確かめて、書き換えられます。書いていただいた内容は Google フォームに保存されます。不具合の修正とアプリの改善にだけ使い、要らなくなったら消します。送った内容を消してほしいときは、もう一度フォームから、どの内容かを書いて送ってください。[Google のプライバシーポリシー](https://policies.google.com/privacy?hl=ja) もご覧ください。

部屋で相手を通報すると、調べられるよう、部屋の番号・相手の名前（名前が出ていなければ二つ名）と猫・日時が入った状態でフォームが開きます。あなたの名前は入りません。送る前に確かめて、書き換えられます。通報は悪用への対応にだけ使い、要らなくなったら消します。

### Apple から届くもの

Apple は開発者に、ダウンロード数などの集計と、iPhone の設定で開発者との共有を選んだ人のクラッシュの記録を渡します。私たちがそこからあなたを特定することはできません。

### 選べること

部屋を使わずに遊べば、対局について iPhone の外へ出るものはありません。外へ出るのは、App Store への確認と、中継への招待の問い合わせだけです。部屋で名前を出したくないときは、部屋に入る前にプロフィールで名前を変えてください。アプリを削除すると、キーチェーンにある招待の鍵のほかは、iPhone に置いたものがすべて消えます。

### お子さまについて

Nyani は、お子さまを含め誰にも、本名・メールアドレス・電話番号・位置情報を求めません。入力する名前はニックネームで、iPhone の中に置きます。部屋では名前の決まりに通したうえで相手に見せ、中継はそれを保存しません。上に書いた短い期間の部屋の記録のほかに中継が持つ ID は、「友だちを誘って Plus」に書いた招待の鍵のハッシュだけです。

### このポリシーの変更

変えるときは、このページと冒頭の日付を更新します。

### 連絡先

フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5 （アプリは Nyani を選んでください）
