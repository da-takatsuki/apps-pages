---
layout: default
title: Linkpoche Privacy Policy
---

# Linkpoche Privacy Policy

Last updated: 2026-10-06

Linkpoche keeps the links you save on your iPhone, and it does not collect any data about you: not for analytics, not for advertising, not in anonymized or aggregated form. It does connect to the internet, though. To show a title and a picture for each link, your iPhone fetches them directly from the sites you saved. This page explains exactly what that involves, item by item, because a sentence saying we care about your privacy doesn't tell you anything.

Linkpoche is published by Daiki Takatsuki. Contact: the feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5

## The short version

- Everything you save is stored on your iPhone. That includes links, screenshots, titles, pictures, notes, pouches and summaries. There is no Linkpoche server, no account and no sign-in.
- To build a preview, your iPhone contacts the site behind each link you save, plus a few services listed below. Those sites receive the request, including your IP address, as they would if you opened the link yourself. Nothing passes through us.
- The AI features use only Apple's on-device model. They do not use Private Cloud Compute.
- Screenshots you add are read on your iPhone and are not uploaded.
- Locked and hidden pouches use Face ID, Touch ID or your passcode through iOS. Linkpoche never receives your face data, fingerprint or passcode.
- Linkpoche Plus is sold by Apple. Linkpoche only learns whether you own it.
- Linkpoche contains no analytics SDK, no crash-reporting SDK and no advertising, and it does no tracking.
- The app sends us nothing about you. There are two exceptions: a message you choose to send through the feedback form, and the reports Apple itself gives developers. See "If you contact us" and "What Apple tells us".

## What stays on your iPhone

The app stores the following in its own storage on your iPhone:

- The links you save, exactly as they arrived.
- What the app fetched for each link: a title, a description (for an X post, the post text), the site name, the author, the publication date, an estimated reading time, one preview picture and the site's icon.
- What you create yourself: pouches (folders), names you give links, notes and pouch icons, including any photo you choose as an icon.
- Summaries written by the on-device AI.
- Screenshots you add: Linkpoche's own copy of the image, the text read from it, and what was found in it (web addresses, @ account names, places and phone numbers). It also keeps a short fingerprint of the original image, so the same screenshot isn't saved twice.
- Which pouches are locked or hidden.
- On iOS 17 or later, an index for searching by meaning (see "Searching by meaning").
- App settings, plus what For you needs to work: which links it showed today, the picks it has planned for the coming days, and the topics it read from your recent links and how close each link is to them, if "Picks from your habits" is on.

The text of an article is read to estimate the reading time and to write a summary. It is kept in memory only and is not saved with the link.

When you save from the share sheet, the start of the page (up to 256 KB) and its preview picture may be saved temporarily in storage that the app shares with its share extension. The app uses them the next time it opens and deletes them after use. Anything left over is deleted after 24 hours. When you share screenshots, the images are copied into that same shared storage. They stay there until Linkpoche next opens and saves its own copy, and are then deleted.

If you back up your iPhone with iCloud Backup or to a computer, iOS includes this app's data in the backup, as it does for most apps. That backup is between you and Apple, and we cannot see it.

## When the app connects to the internet, and to whom

### When

- After you save a link, whether from the share sheet, by pasting, or with the Shortcuts action.
- Right after you share a link, the share extension starts fetching the page and its preview picture. It may also ask iOS's background download service to fetch them, so the preview is ready when you open the app.
- If a fetch fails right after saving, the app tries once more a few seconds later.
- When a screenshot you add contains a web address, your iPhone fetches that page, as it does for any link you save.
- When you tap Fetch again.
- While the app is open, it goes back over links you have already saved, one at a time, to read the article text for reading time and summaries. When it writes a longer summary for a link whose text is no longer in memory, it reads that page again.

Saving a link is what starts the fetch. There is no setting to save a link without fetching its preview.

### To whom

1. **The site of the link you saved, and any site it redirects to.** Your iPhone requests the page through Apple's LinkPresentation framework, the same system feature Safari and Messages use for link previews. The app also reads the page's HTML itself: the first 64 KB, or up to 1.5 MB for pages that may be articles.
2. **Wherever that page points for its preview picture and its icon.** These are often on a different company's server, such as a content delivery network. If the page does not name an icon, the app asks the site for `/favicon.ico`.
3. **Four services, for their own links.** For a YouTube video link, the app asks YouTube's official embed service (`www.youtube.com/oembed`) for the video title and channel. For an X post link, it asks X's official embed service (`publish.x.com/oembed`) for the post text, author and date. For an Instagram post, it reads the post's public embed page (`www.instagram.com/p/<code>/embed/captioned/`), and for a Threads post, the post's public embed page (`www.threads.com/@<user>/post/<code>/embed`), for the caption, account name and picture. None of these needs a sign-in or a key.

   The request to X includes X's do-not-track option (`dnt=true`). That option only asks X not to use the request for personalized suggestions and ads. The request itself, including your IP address and the link, still reaches X.
4. **For an X post that contains a link:** X's link shortener (`t.co`), to learn where the link leads, and then that destination site, as in 1 and 2.
5. **Apple, for language files (iOS 17 or later).** Searching by meaning uses language files that iOS downloads from Apple the first time they are needed. iOS makes that download, not Linkpoche, and none of your links, screenshots or searches are sent with it. Apple's privacy policy covers it.

### What they receive

- The full address of the link, including any parameters in it. The embed services in item 3 receive the link as part of their own address.
- Your IP address, as with any internet connection.
- Standard request headers. The User-Agent describes the software making the request, and some requests name Linkpoche in it. Requests for pages also send Accept-Language, which lists the languages set on your iPhone so the site can answer in your language.

They do not receive an account, an identifier, your notes, your other links or anything else you saved, because the app does not send them. What a site does with a request it receives is up to that site and its own privacy policy. It is the same kind of request a browser makes when you open the link.

"No tracking" on this page means that we, the developer, do not track you. We cannot control what a site, X, Google (YouTube) or Meta (Instagram and Threads) keeps in its own server logs.

When you open a link, the app hands it to your browser or to the app that handles it. From there, that app makes the connection.

## On-device AI

On iPhones where Apple Intelligence is available and turned on (iOS 26 or later), Linkpoche uses it to write short summaries, write longer summaries in the AI tab, suggest a pouch for a new link, pick links based on your recent interests, write a short title for a screenshot, and suggest up to three related words when you search.

- It uses only the on-device model in Apple's Foundation Models framework. It does not use Private Cloud Compute, so the AI features never send your links anywhere.
- What the model reads: a link's title, description and the start of its article text; the text read from a screenshot; the words you type in search; your pouch names and the titles of a few links in each; and the titles, site names and summaries of links you saved recently.
- Measuring how close a link is to your interests uses Apple's NaturalLanguage framework, which also runs on your iPhone.
- The On-device AI section in Settings has three switches: Write summaries, Light up where it goes and Picks from your habits. All three are on by default. Turning off Write summaries stops new summaries and hides the ones already written. Turning off Picks from your habits deletes the topics and closeness scores from your iPhone.
- Turning off Write summaries also stops the on-device AI from writing titles for new screenshots. Related search words aren't covered by these three switches. They appear only while Apple Intelligence is available and turned on.

## Screenshots

You can add screenshots by sharing them to Linkpoche (up to 10 at a time) or with Add screenshots, which opens iOS's photo picker. Linkpoche receives only the images you choose. It doesn't ask for access to your photo library.

Everything below happens on your iPhone:

- Linkpoche makes its own copy of the image, resized to 1,200 pixels on the long side and saved without the details stored in the image file, such as location and the time it was taken.
- It reads the text (Japanese and English), QR codes, web addresses, phone numbers and addresses with Apple's Vision and data detection, which run on your iPhone.
- On iPhones with Apple Intelligence, the on-device model may write a title from the text it read (see "On-device AI").

Screenshots are never uploaded. The copy, its text and what was found in it are stored with your other items, appear in search and are included in Export. If a web address is found, your iPhone fetches that page as it does for any link you save. Live Text in the full-screen view is iOS's own feature and runs on your iPhone.

The original stays in Photos, where it can show up in Photos search and widgets. Deleting a screenshot in Linkpoche doesn't delete it from Photos.

## Searching by meaning

On iOS 17 or later, search can also find links close in meaning, not only exact words. Linkpoche builds an index for this on your iPhone with Apple's NaturalLanguage framework. The index is kept in the app's cache folder, which iOS doesn't include in backups, and it isn't included in Export.

The first time, iOS downloads the language files it needs from Apple (see item 5 under "To whom"). Until they are ready, search finds exact words only.

## Locked and hidden pouches, Face ID and Touch ID

When you lock a pouch, open a locked pouch or a link in one, remove a lock, show hidden pouches, stop hiding a pouch, or delete or export locked and hidden pouches, Linkpoche asks iOS to confirm it's the device owner with Face ID, Touch ID or your passcode (Apple's LocalAuthentication).

- iOS does the check and tells Linkpoche only whether it succeeded. Linkpoche never receives your face data, fingerprint or passcode, and nothing about the check leaves your iPhone.
- Which pouches are locked or hidden is stored with your pouches on your iPhone.
- A lock is a check Linkpoche makes before it shows a pouch. The links inside are stored the same way as in any other pouch, and they are included in your iPhone backup and in Export. Anyone who can unlock your iPhone can open a locked pouch. The support page lists what locks and hiding don't do.

## Linkpoche Plus (in-app purchase)

Linkpoche Plus is an optional one-time purchase. Apple sells it and handles the payment with your Apple Account. Linkpoche asks the App Store on your iPhone whether you own Plus. It does not receive your payment details, name or email address. The sales reports Apple gives us are described under "What Apple tells us".

## Home Screen widget and Spotlight

- **Widget.** For the Today's rediscoveries widget, the app writes a copy of the upcoming picks into storage that the app shares with the widget. For each link, the copy holds the title, the site's host name, the pouch name, the date you saved it and a small picture. It does not include the link's address, your notes, the description or the AI summary. For a screenshot, the small picture is a reduced copy of the screenshot. Anyone who can see your Home Screen can see what the widget shows.
- **Spotlight.** Linkpoche adds your saved links to iOS's on-device search, but not the ones in Recently Deleted. Each entry holds the title (or host name), pouch name, site name or host name, author, the short AI summary if one exists, and a small picture. It does not include the link's address or your notes. Apple says this index stays on your device, is not shared with Apple and is not synced to your other devices. When you delete a link, its entry is removed.

## Clipboard

To offer a paste shortcut, the app asks iOS only whether the clipboard appears to hold a web link. iOS answers this without showing the app what the clipboard contains. The app reads the clipboard only when you tap to paste, and iOS asks your permission at that moment. The Shortcuts action receives the link from your shortcut; the app itself does not touch the clipboard.

## Export and import

- Export puts your links, everything saved with them (including notes and summaries), your screenshots, your pouches and their pictures into a zip file and opens the share sheet. Locked and hidden pouches are included, and the zip file itself isn't locked. You choose where it goes. A copy stays in the app's temporary folder until your next export replaces it or iOS clears temporary files.
- Import reads a zip file you choose. The app deletes its own copy of the file after reading it.

## Deleting

- A deleted link moves to Recently Deleted with its pictures. Recently Deleted holds up to 50 links. When a 51st arrives, the oldest is deleted permanently. "Delete all permanently" empties it straight away.
- Settings has "Delete all saved images", which removes every stored link picture and icon but keeps the links. Screenshots you added are not removed, because the screenshot is the item itself. Delete a screenshot like any link.
- Deleting the app removes its data from your iPhone. Backups you already made keep what they contain until they are replaced.

## No third parties in the app

Linkpoche contains no analytics, attribution, advertising, crash-reporting or A/B-testing SDK. It shows no ads, and no data is used for tracking as Apple defines it.

It is built with open-source Flutter packages, which is normal for an iOS app. They make the preview requests described above, parse web pages, store data on the device, open links and read the app version. None of them is an analytics or advertising component.

## If you contact us

The feedback form is the only way we receive anything from you, and we receive only what is in it.

- The form asks for three things and nothing else: a type of feedback, your message, and the app and iOS versions. It does not ask for your name or email address. If you open the form from inside the app, the version numbers are already filled in, and you can see them before you send.
- It is a Google Form, hosted by Google. What you submit is sent to Google's servers and stored in our Google account, where we read it. What Google does as the host of that page is covered by Google's privacy policy at https://policies.google.com/privacy
- The form does not ask you to sign in, and it is not set to collect the Google account of whoever fills it in.
- Because the form collects no contact details, we cannot reply to you individually. We read every message and use it only to fix problems and improve the app. We do not share what you send with anyone.
- We delete feedback once it is resolved and no longer needed to handle the same problem again.
- Please do not include links you want to keep private. We do not need them to answer most questions.

## What Apple tells us

- Apple gives every developer sales and download reports for their own app: counts by country and date. They do not identify anyone.
- If you have turned on sharing with app developers in iOS Settings (Privacy & Security > Analytics & Improvements), Apple includes your device in the usage figures it shows us in App Store Connect, and may share crash reports with us. We see totals, not people. This is Apple's reporting to developers, not data collected by the app. You can turn it off at any time in that setting.
- The app may ask iOS to show Apple's rating prompt. Whether it appears is up to iOS. Any rating or review you leave goes to Apple and appears on the App Store.

## Children

The app collects nothing from anyone, at any age.

## Your rights

Everything the app stores is on your iPhone, and you can view, change, export or delete it in the app. We hold nothing from the app, so there is nothing for us to access, correct or delete. The one thing we may hold is a message you sent through the feedback form. If you ask us to delete it, we will. For what a website did with a request from your iPhone, contact that website.

## This website (linkpoche.pages.dev)

This section covers the Linkpoche website at https://linkpoche.pages.dev, not the app. The app does not use it.

- The website is hosted on Cloudflare Pages. As with any website, Cloudflare receives your request, including your IP address and browser details, to deliver the page. Cloudflare's privacy policy covers this: https://www.cloudflare.com/privacypolicy/
- The website uses Cloudflare Web Analytics to count visits. It loads a small script from Cloudflare that reports the page you viewed, the page that linked to it, your browser and device type, your country, and how fast the page loaded. Cloudflare says it uses no cookies or local storage for this and does not fingerprint visitors by IP address or User-Agent. We see only totals, such as visits per page and per country, never individual visitors.
- The website sets no cookies, has no ads, and has no sign-in or forms.
- Links to the App Store include a campaign label (for example `ct=lp-en-top-hero`) so App Store Connect can count downloads that came from the website. Apple reports these to us only as totals.

## Changes to this policy

If this policy changes, the new version will be posted here with a new date at the top, and the App Store listing will be updated in the same release. We will not start collecting data in a silent update.

## Contact

Feedback form: https://forms.gle/GqJSQ4cF1YpSt5vx5

---

## 日本語

最終更新日: 2026-10-06

Linkpoche は、保存したリンクを iPhone の中に置いておくアプリです。お使いの方に関するデータは集めていません。分析のためにも、広告のためにも集めず、匿名化や集計をした形でも集めません。ただし、インターネットにはつながります。リンクごとに題と絵を出すため、保存したサイトから iPhone が直接取りにいきます。それが何を意味するのかを、以下に項目ごとに書きます。「プライバシーを大切にしています」という一文では、何も伝わらないからです。

公開者: Daiki Takatsuki。連絡先: ご意見フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5

### 要約

- 保存したものは、すべて iPhone の中にあります。リンク、スクショ、題、絵、メモ、ポーチ、概要が含まれます。Linkpoche のサーバーはなく、アカウントもサインインもありません。
- プレビューを作るため、保存したリンクのサイトと、下に挙げるいくつかのサービスに iPhone が直接つなぎます。相手のサイトには、ご自分でリンクを開いたときと同じように、IP アドレスを含むリクエストが届きます。私たちを経由するものはありません。
- AI の機能が使うのは、Apple の端末内のモデルだけです。Private Cloud Compute は使いません。
- 入れたスクショは iPhone の中で読み取り、アップロードしません。
- 鍵付き・隠しのポーチは、iOS を通して Face ID・Touch ID・パスコードを使います。顔や指紋のデータ、パスコードが Linkpoche に届くことはありません。
- Linkpoche Plus を販売しているのは Apple です。Linkpoche が知るのは、Plus を持っているかどうかだけです。
- 分析の SDK、クラッシュ報告の SDK、広告は入っておらず、トラッキングもしません。
- アプリからあなたの情報が私たちに届くことはありません。例外は 2 つです。ご自分でフォームから送ったお便りと、Apple が開発者に渡す報告です（「お問い合わせについて」「Apple から届くもの」を参照）。

### iPhone の中に置くもの

アプリは、iPhone 上のアプリ専用の置き場に次のものを保存します。

- 保存したリンク（届いたままの形）
- リンクごとに取得したもの: 題、説明文（X の投稿なら本文）、サイト名、著者、公開日、読む時間の目安、プレビューの絵 1 枚、サイトのアイコン
- ご自分で作ったもの: ポーチ（フォルダ）、リンクに付けた名前、メモ、ポーチの印（印に選んだ写真を含む）
- 端末内 AI が作った概要
- 入れたスクショ: Linkpoche が作った画像の写し、そこから読み取った文字、見つかったもの（Web のアドレス・@ で始まるアカウント名・場所・電話番号）。同じスクショを二重に保存しないよう、元の画像の短い指紋も持ちます
- どのポーチに鍵をかけているか、どのポーチを隠しているか
- iOS 17 以降では、意味で探すための索引（「意味で探す」を参照）
- アプリの設定と、For you の動作に必要な記録。今日出したリンク、この先の数日ぶんの予定、「傾向でおすすめ」がオンなら最近のリンクから読んだ話題と、各リンクがその話題にどれだけ近いかです

記事の本文は、読む時間の目安と概要を作るために読みます。読んだ本文はメモリの中に置くだけで、リンクと一緒には保存しません。

共有シートから保存したときは、ページの先頭（256 KB まで）とプレビューの絵を、アプリと共有拡張が一緒に使う置き場に一時的に置くことがあります。次にアプリを開いたときに使い、使い終わったら消します。残ったものも 24 時間で消えます。スクショを共有したときは、画像を同じ置き場に写します。次に Linkpoche を開いて写しを作るまでそこに置き、作り終えたら消します。

iCloud バックアップやコンピュータで iPhone をバックアップしている場合、iOS はほとんどのアプリと同じように、このアプリのデータもバックアップに含めます。そのバックアップはお使いの方と Apple のあいだのもので、私たちからは見えません。

### いつ、どこへつなぐか

#### いつ

- リンクを保存したあと（共有シート、貼り付け、ショートカットのいずれでも）
- 共有した直後に、共有拡張がページとプレビューの絵を取りにいきます。アプリを開いたときにプレビューがそろっているよう、iOS のバックグラウンドのダウンロードに取得を頼むこともあります
- 保存した直後の取得に失敗したときは、数秒後に 1 回だけやり直します
- 入れたスクショに Web のアドレスが書いてあったとき。保存したほかのリンクと同じように、iPhone がそのページを取りにいきます
- 「取り直す」を押したとき
- アプリを開いているあいだ、保存済みのリンクを 1 件ずつ読み直して、読む時間と概要のための本文を取ります。本文がもうメモリにないリンクの長い概要を作るときも、そのページをもう一度読みます

取得のきっかけはリンクの保存です。プレビューを取らずにリンクだけ保存する設定はありません。

#### どこへ

1. **保存したリンクのサイトと、そこから転送された先のサイト。** Apple の LinkPresentation を通してページを取りにいきます。Safari やメッセージがリンクのプレビューに使うのと同じ、iOS の標準機能です。アプリ自身もページの HTML を読みます。読むのは先頭 64 KB までで、記事かもしれないページだけ 1.5 MB まで読みます。
2. **そのページが、プレビューの絵とアイコンの置き場として指している先。** コンテンツ配信網など、別の会社のサーバーであることがよくあります。アイコンを指定していないページには、そのサイトの `/favicon.ico` を取りにいきます。
3. **4 つのサービス（それぞれのリンクのときだけ）。** YouTube の動画リンクでは、YouTube 公式の埋め込みの窓口（`www.youtube.com/oembed`）に動画の題とチャンネルを尋ねます。X の投稿リンクでは、X 公式の埋め込みの窓口（`publish.x.com/oembed`）に投稿の本文・投稿者・日付を尋ねます。Instagram の投稿では投稿の公開の埋め込みページ（`www.instagram.com/p/<code>/embed/captioned/`）を、Threads の投稿では投稿の公開の埋め込みページ（`www.threads.com/@<user>/post/<code>/embed`）を読み、キャプション・アカウント名・写真を取ります。どれもサインインや鍵は要りません。

   X への問い合わせには、X の追跡拒否の指定（`dnt=true`）を付けています。この指定は、個人向けのおすすめや広告にその問い合わせを使わないよう X に求めるだけです。IP アドレスとリンクを含む問い合わせそのものは X に届きます。
4. **リンクを含む X の投稿のとき:** 行き先を知るために X の短縮 URL の窓口（`t.co`）につなぎ、そのあと行き先のサイトに 1・2 と同じようにつなぎます。
5. **Apple（言語のデータ。iOS 17 以降）。** 意味で探すには、iOS が最初に必要になったときに Apple からダウンロードする言語のデータを使います。ダウンロードするのは iOS で、Linkpoche ではありません。そのときにリンク・スクショ・検索した言葉を送ることはありません。扱いは Apple のプライバシーポリシーに従います。

#### 相手に届くもの

- リンクのアドレス全体。含まれるパラメータもすべて届きます。3 の埋め込みの窓口には、リンクが問い合わせのアドレスの一部として届きます。
- IP アドレス。インターネットにつなぐときは、どの通信でも届くものです。
- 通信の標準のヘッダ。User-Agent にはリクエストを送るソフトウェアの名前が入り、リクエストによっては Linkpoche の名前も入ります。ページを取るリクエストには Accept-Language も付けます。iPhone に設定している言語の一覧で、相手がその言語で返せるようにするためのものです。

アカウント、識別子、メモ、ほかのリンクなど、保存したものは相手に届きません。アプリが送っていないからです。届いたリクエストを相手のサイトがどう扱うかは、そのサイトとそのサイトのプライバシーポリシーによります。ブラウザでリンクを開いたときと同じ種類のリクエストです。

このページの「トラッキングしません」は、開発者である私たちがあなたを追跡しないという意味です。相手のサイトや、X・Google（YouTube）・Meta（Instagram・Threads）が自分のサーバーの記録に何を残すかは、私たちには決められません。

リンクを開くと、アプリはそのリンクをブラウザか、そのリンクを扱うアプリに渡します。そこから先の通信はそのアプリが行います。

### 端末内 AI

Apple Intelligence が使えて、オンになっている iPhone（iOS 26 以降）では、Linkpoche はそれを使って短い概要と AI タブの長い概要を作り、新しいリンクの行き先のポーチを示し、最近の関心からおすすめを選び、スクショに短いタイトルを付け、検索のときに近い言葉を 3 つまで挙げます。

- 使うのは Apple の Foundation Models の端末内のモデルだけで、Private Cloud Compute は使いません。AI の機能がリンクを外へ送ることはありません。
- モデルが読むもの: リンクの題・説明文・本文の先頭、スクショから読み取った文字、検索に打った言葉、ポーチの名前と各ポーチのリンクの題を数件、最近保存したリンクの題・サイト名・概要です。
- リンクが関心にどれだけ近いかは、Apple の NaturalLanguage で測ります。これも iPhone の中で動きます。
- 設定の「端末内 AI」にスイッチが 3 つあります（「概要を作る」「行き先を照らす」「傾向でおすすめ」）。どれも最初はオンです。「概要を作る」を切ると、新しい概要を作らず、作った概要も表示しなくなります。「傾向でおすすめ」を切ると、話題と近さの記録を iPhone から消します。
- 「概要を作る」を切ると、新しく入れたスクショのタイトルも端末内 AI では作りません。検索の近い言葉は、この 3 つの切り替えの対象ではありません。Apple Intelligence が使えて、オンになっているときだけ出ます。

### スクショ

スクショは、Linkpoche に共有する（一度に 10 枚まで）か、「スクショを入れる」で iOS の写真の選択画面から入れます。Linkpoche が受け取るのは、選んだ画像だけです。写真ライブラリへのアクセスは求めません。

次のことは、すべて iPhone の中で行います。

- Linkpoche 用の写しを作ります。長辺 1,200 ピクセルに縮め、位置情報や撮った日時など、画像ファイルに入っている情報を外して保存します。
- 文字（日本語と英語）・QR コード・Web のアドレス・電話番号・住所を、iPhone の中で動く Apple の Vision とデータ検出で読み取ります。
- Apple Intelligence に対応した iPhone では、読み取った文字から端末内のモデルがタイトルを付けることがあります（「端末内 AI」を参照）。

スクショをアップロードすることはありません。写しと読み取った文字・見つかったものは、ほかの項目と一緒に保存され、検索に出て、書き出しにも入ります。Web のアドレスが見つかったときは、保存したほかのリンクと同じように、iPhone がそのページを取りにいきます。全面の画面の Live Text は iOS の機能で、iPhone の中で動きます。

元のスクショは写真アプリに残り、写真の検索やウィジェットに出ることがあります。Linkpoche でスクショを消しても、写真アプリからは消えません。

### 意味で探す

iOS 17 以降では、言葉がぴったり合わなくても、意味の近いリンクも探せます。そのための索引は、Apple の NaturalLanguage を使って iPhone の中で作ります。索引はアプリのキャッシュの置き場に置き、iOS はここをバックアップに含めません。書き出しにも入れません。

初回は、iOS が必要な言語のデータを Apple からダウンロードします（「どこへ」の 5）。準備ができるまでは、言葉が合うものだけを探します。

### 鍵付き・隠しのポーチと Face ID・Touch ID

ポーチに鍵をかける、鍵付きのポーチやその中のリンクを開く、鍵を外す、隠しポーチを表示する、隠すのをやめる、鍵付きや隠しのポーチを消す・書き出す、ときに、Linkpoche は Face ID・Touch ID・パスコードで端末の持ち主かどうかを確かめるよう iOS に頼みます（Apple の LocalAuthentication）。

- 確認は iOS が行い、Linkpoche に伝わるのは通ったかどうかだけです。顔や指紋のデータ、パスコードが Linkpoche に届くことはなく、確認について iPhone の外へ出るものもありません。
- どのポーチに鍵をかけているか・隠しているかは、ポーチと一緒に iPhone の中に保存します。
- 鍵は、Linkpoche がポーチを見せる前に行う確認です。中のリンクはほかのポーチと同じ形で保存され、iPhone のバックアップと書き出しにも入ります。iPhone のロックを解除できる人は、鍵付きのポーチも開けます。鍵と隠しにできないことは、サポートページにまとめています。

### Linkpoche Plus（App 内課金）

Linkpoche Plus は、必要な人だけが買う 1 回きりの購入です。販売しているのは Apple で、支払いは Apple アカウントで Apple が扱います。Linkpoche は、Plus を持っているかを iPhone の App Store の仕組みに尋ねるだけで、支払いの情報・名前・メールアドレスは受け取りません。Apple から届く販売の報告は「Apple から届くもの」に書いています。

### ホーム画面のウィジェットと Spotlight

- **ウィジェット。** 「今日の再会」ウィジェットのために、アプリはこの先のおすすめの写しを、ウィジェットと一緒に使う置き場に書きます。写しに入るのは、リンクごとの題、サイトのホスト名、ポーチ名、保存した日付、小さな絵です。リンクのアドレス、メモ、説明文、AI の概要は入れません。スクショの場合、小さな絵はスクショを縮めた写しです。ウィジェットの中身は、ホーム画面が見える人なら誰でも見られます。
- **Spotlight。** Linkpoche は保存したリンクを iOS の端末内検索に載せます。「最近削除した項目」のリンクは載せません。1 件に入るのは、題（なければホスト名）、ポーチ名、サイト名またはホスト名、著者、短い AI の概要（あれば）、小さな絵です。リンクのアドレスとメモは入れません。Apple によると、この検索用のデータは端末の中にとどまり、Apple には共有されず、ほかの端末とも同期されません。リンクを削除すると、Spotlight からも外れます。

### クリップボード

貼り付けの近道を出すため、アプリはクリップボードに「Web のリンクらしきものがあるか」だけを iOS に尋ねます。iOS は、クリップボードの中身をアプリに見せずにこれに答えます。中身を読むのは貼り付けを押したときだけで、そのとき iOS が許可を求めます。ショートカットのアクションはショートカットからリンクを受け取るので、アプリ自身はクリップボードに触れません。

### 書き出しと取り込み

- 書き出しは、リンクと一緒に保存しているものすべて（メモと概要を含む）、スクショ、ポーチ、絵を zip にまとめ、共有シートを開きます。鍵付き・隠しのポーチも入り、zip そのものには鍵がかかりません。行き先はご自分で選びます。控えは、次に書き出して置き換わるか、iOS が一時ファイルを片付けるまで、アプリの一時フォルダに残ります。
- 取り込みは、ご自分で選んだ zip を読みます。読み終えたら、アプリが持っている複製を消します。

### 削除

- 削除したリンクは、絵を持ったまま「最近削除した項目」に移ります。「最近削除した項目」には 50 件まで入り、51 件目が入ると、いちばん古いものを完全に削除します。「すべて完全に削除」を押すと、その場で空になります。
- 設定の「保存した画像をすべて消す」を押すと、リンクは残したまま、保存したリンクの絵とアイコンをすべて消します。入れたスクショは消しません（スクショはその項目そのものだからです）。スクショはリンクと同じように削除してください。
- アプリを削除すると、アプリのデータは iPhone から消えます。すでに作ったバックアップの中身は、そのバックアップが置き換わるまで残ります。

### アプリに第三者は入っていない

分析、広告の効果計測、広告、クラッシュ報告、A/B テストの SDK は入っていません。広告は出さず、Apple の定義するトラッキングにデータを使うこともありません。

iOS アプリとして一般的な、オープンソースの Flutter パッケージで作っています。上に書いたプレビューの取得、Web ページの解析、端末内の保存、リンクを開くこと、アプリの版の読み取りに使っています。分析や広告の部品はありません。

### お問い合わせについて

私たちに何かが届く経路は、ご意見フォームだけです。届くのは、フォームに入っているものだけです。

- フォームの項目は、ご意見の種類、内容、アプリと iOS の版の 3 つだけです。お名前やメールアドレスはお聞きしません。アプリから開くと、版は最初から入っていて、送る前に確かめられます。
- フォームは Google が提供する Google フォームです。送った内容は Google のサーバーに送られ、私たちの Google アカウントに保存され、私たちはそこで読みます。ページの提供者としての Google の扱いは、Google のプライバシーポリシー https://policies.google.com/privacy に従います。
- フォームはサインインを求めず、記入した人の Google アカウントを集める設定にもしていません。
- 連絡先をお聞きしないため、個別にお返事することはできません。いただいた内容はすべて読み、不具合の修正とアプリの改善のためだけに使います。送られた内容をほかの誰かに渡すことはありません。
- お便りは、解決して同じ問題の対応にもう要らなくなった時点で削除します。
- 人に見せたくないリンクは書かないでください。ほとんどのご質問は、リンクがなくてもお答えできます。

### Apple から届くもの

- Apple は、どの開発者にも自分のアプリの販売とダウンロードの報告を渡します。国別・日付別の件数で、個人は特定されません。
- iOS の設定（プライバシーとセキュリティ > 解析および改善）で App デベロッパとの共有をオンにしている場合、Apple は App Store Connect で私たちに見せる利用状況の数字にその端末を含め、クラッシュの報告を共有することもあります。私たちに見えるのは合計で、個人ではありません。これは Apple から開発者への報告で、アプリが集めたデータではありません。この共有は、その設定でいつでも切れます。
- アプリは iOS に Apple の評価の画面を出すよう頼むことがあります。実際に出るかどうかは iOS が決めます。付けた評価やレビューは Apple に届き、App Store に表示されます。

### お子さまについて

年齢にかかわらず、アプリは誰からも何も集めません。

### あなたの権利

アプリが保存するものはすべて iPhone の中にあり、アプリの中で見る・直す・書き出す・消すことができます。アプリから私たちが預かっているものはないので、開示・訂正・削除の対象もありません。例外は、フォームから送られたお便りです。削除をご希望の場合は削除します。iPhone から届いたリクエストをサイトがどう扱ったかについては、そのサイトにお問い合わせください。

### この Web サイト（linkpoche.pages.dev）

この節は、アプリではなく Linkpoche の Web サイト https://linkpoche.pages.dev についてです。アプリはこのサイトを使いません。

- サイトは Cloudflare Pages に置いています。ほかの Web サイトと同じく、ページを届けるために、Cloudflare はあなたの IP アドレスやブラウザの情報を含む要求を受け取ります。その扱いは Cloudflare のプライバシーポリシーに従います: https://www.cloudflare.com/privacypolicy/
- 訪問数を数えるため、Cloudflare Web Analytics を使っています。Cloudflare の小さなスクリプトを読み込み、見たページ、そのページへのリンク元、ブラウザと端末の種類、国、ページの表示にかかった時間を送ります。Cloudflare によれば、このためにクッキーや端末内の保存領域は使わず、IP アドレスや User-Agent で訪問者を識別することもしません。私たちが見るのはページごと・国ごとの訪問数などの合計だけで、一人ひとりの訪問者は見えません。
- サイトはクッキーを置かず、広告もなく、ログインや入力フォームもありません。
- App Store へのリンクには、サイトから来たダウンロードを App Store Connect で数えるための印（例 `ct=lp-ja-top-hero`）を付けています。Apple から届くのは合計の数だけです。

### このポリシーの変更

変更したときは、新しい日付を付けてこのページに載せ、同じリリースで App Store の掲載情報も更新します。黙ってアップデートし、データを集め始めることはしません。

### 連絡先

ご意見フォーム: https://forms.gle/GqJSQ4cF1YpSt5vx5
