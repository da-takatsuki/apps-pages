---
layout: default
title: Linkpoche Privacy Policy
---

# Linkpoche Privacy Policy

Last updated: 2026-09-26

Linkpoche keeps the links you save on your iPhone, and it does not collect any data about you: not for analytics, not for advertising, not in anonymized or aggregated form. It does connect to the internet, though. To show a title and a picture for each link, your iPhone fetches them directly from the sites you saved. This page explains exactly what that involves, item by item, because a sentence saying we care about your privacy doesn't tell you anything.

Linkpoche is published by Daiki Takatsuki. Contact: the feedback form at https://forms.gle/GqJSQ4cF1YpSt5vx5

## The short version

- Everything you save is stored on your iPhone. That includes links, titles, pictures, notes, pouches and summaries. There is no Linkpoche server, no account and no sign-in.
- To build a preview, your iPhone contacts the site behind each link you save, plus a few services listed below. Those sites receive the request, including your IP address, as they would if you opened the link yourself. Nothing passes through us.
- The AI features use only Apple's on-device model. They do not use Private Cloud Compute.
- Linkpoche contains no analytics SDK, no crash-reporting SDK and no advertising, and it does no tracking.
- The app sends us nothing about you. There are two exceptions: a message you choose to send through the feedback form, and the reports Apple itself gives developers. See "If you contact us" and "What Apple tells us".

## What stays on your iPhone

The app stores the following in its own storage on your iPhone:

- The links you save, exactly as they arrived.
- What the app fetched for each link: a title, a description (for an X post, the post text), the site name, the author, the publication date, an estimated reading time, one preview picture and the site's icon.
- What you create yourself: pouches (folders), names you give links, notes and pouch icons, including any photo you choose as an icon.
- Summaries written by the on-device AI.
- App settings, plus what For you needs to work: which links it showed today, the picks it has planned for the coming days, and the topics it read from your recent links and how close each link is to them, if "Picks from your habits" is on.

The text of an article is read to estimate the reading time and to write a summary. It is kept in memory only and is not saved with the link.

When you save from the share sheet, the start of the page (up to 256 KB) and its preview picture may be saved temporarily in storage that the app shares with its share extension. The app uses them the next time it opens and deletes them after use. Anything left over is deleted after 24 hours.

If you back up your iPhone with iCloud Backup or to a computer, iOS includes this app's data in the backup, as it does for most apps. That backup is between you and Apple, and we cannot see it.

## When the app connects to the internet, and to whom

### When

- After you save a link, whether from the share sheet, by pasting, or with the Shortcuts action.
- Right after you share a link, the share extension starts fetching the page and its preview picture. It may also ask iOS's background download service to fetch them, so the preview is ready when you open the app.
- If a fetch fails right after saving, the app tries once more a few seconds later.
- When you tap Fetch again.
- While the app is open, it goes back over links you have already saved, one at a time, to read the article text for reading time and summaries. When it writes a longer summary for a link whose text is no longer in memory, it reads that page again.

Saving a link is what starts the fetch. There is no setting to save a link without fetching its preview.

### To whom

1. **The site of the link you saved, and any site it redirects to.** Your iPhone requests the page through Apple's LinkPresentation framework, the same system feature Safari and Messages use for link previews. The app also reads the page's HTML itself: the first 64 KB, or up to 1.5 MB for pages that may be articles.
2. **Wherever that page points for its preview picture and its icon.** These are often on a different company's server, such as a content delivery network. If the page does not name an icon, the app asks the site for `/favicon.ico`.
3. **YouTube and X, for their own links.** For a YouTube video link, the app asks YouTube's official embed service (`www.youtube.com/oembed`) for the video title and channel. For an X post link, it asks X's official embed service (`publish.x.com/oembed`) for the post text, author and date. The request to X includes X's do-not-track option (`dnt=true`).
4. **For an X post that contains a link:** X's link shortener (`t.co`), to learn where the link leads, and then that destination site, as in 1 and 2.

### What they receive

- The full address of the link, including any parameters in it. The embed services in item 3 receive the link as part of their own address.
- Your IP address, as with any internet connection.
- Standard request headers. The User-Agent describes the software making the request, and some requests name Linkpoche in it. Requests for pages also send Accept-Language, which lists the languages set on your iPhone so the site can answer in your language.

They do not receive an account, an identifier, your notes, your other links or anything else you saved, because the app does not send them. What a site does with a request it receives is up to that site and its own privacy policy. It is the same kind of request a browser makes when you open the link.

When you open a link, the app hands it to your browser or to the app that handles it. From there, that app makes the connection.

## On-device AI

On iPhones where Apple Intelligence is available and turned on (iOS 26 or later), Linkpoche uses it to write short summaries, write longer summaries in the AI tab, suggest a pouch for a new link, and pick links based on your recent interests.

- It uses only the on-device model in Apple's Foundation Models framework. It does not use Private Cloud Compute, so the AI features never send your links anywhere.
- What the model reads: a link's title, description and the start of its article text; your pouch names and the titles of a few links in each; and the titles, site names and summaries of links you saved recently.
- Measuring how close a link is to your interests uses Apple's NaturalLanguage framework, which also runs on your iPhone.
- The On-device AI section in Settings has three switches: Write summaries, Light up where it goes and Picks from your habits. All three are on by default. Turning off Write summaries stops new summaries and hides the ones already written. Turning off Picks from your habits deletes the topics and closeness scores from your iPhone.

## Home Screen widget and Spotlight

- **Widget.** For the Today's rediscoveries widget, the app writes a copy of the upcoming picks into storage that the app shares with the widget. For each link, the copy holds the title, the site's host name, the pouch name, the date you saved it and a small picture. It does not include the link's address, your notes, the description or the AI summary. Anyone who can see your Home Screen can see what the widget shows.
- **Spotlight.** Linkpoche adds your saved links to iOS's on-device search, but not the ones in Recently Deleted. Each entry holds the title (or host name), pouch name, site name or host name, author, the short AI summary if one exists, and a small picture. It does not include the link's address or your notes. Apple says this index stays on your device, is not shared with Apple and is not synced to your other devices. When you delete a link, its entry is removed.

## Clipboard

To offer a paste shortcut, the app asks iOS only whether the clipboard appears to hold a web link. iOS answers this without showing the app what the clipboard contains. The app reads the clipboard only when you tap to paste, and iOS asks your permission at that moment. The Shortcuts action receives the link from your shortcut; the app itself does not touch the clipboard.

## Export and import

- Export puts your links, everything saved with them (including notes and summaries), your pouches and their pictures into a zip file and opens the share sheet. You choose where it goes. A copy stays in the app's temporary folder until your next export replaces it or iOS clears temporary files.
- Import reads a zip file you choose. The app deletes its own copy of the file after reading it.

## Deleting

- A deleted link moves to Recently Deleted with its pictures. Recently Deleted holds up to 50 links. When a 51st arrives, the oldest is deleted permanently. "Delete all permanently" empties it straight away.
- Settings has "Delete all saved images", which removes every stored picture and icon but keeps the links.
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

## Changes to this policy

If this policy changes, the new version will be posted here with a new date at the top, and the App Store listing will be updated in the same release. We will not start collecting data in a silent update.

## Contact

Feedback form: https://forms.gle/GqJSQ4cF1YpSt5vx5

---

## 日本語

最終更新日: 2026-09-26

Linkpoche は、保存したリンクを iPhone の中に置いておくアプリです。お使いの方に関するデータは集めていません。分析のためにも、広告のためにも集めず、匿名化や集計をした形でも集めません。ただし、インターネットにはつながります。リンクごとに題と絵を出すため、保存したサイトから iPhone が直接取りにいきます。それが何を意味するのかを、以下に項目ごとに書きます。「プライバシーを大切にしています」という一文では、何も伝わらないからです。

公開者: Daiki Takatsuki。連絡先: ご意見フォーム https://forms.gle/GqJSQ4cF1YpSt5vx5

### 要約

- 保存したものは、すべて iPhone の中にあります。リンク、題、絵、メモ、ポーチ、概要が含まれます。Linkpoche のサーバーはなく、アカウントもサインインもありません。
- プレビューを作るため、保存したリンクのサイトと、下に挙げるいくつかのサービスに iPhone が直接つなぎます。相手のサイトには、ご自分でリンクを開いたときと同じように、IP アドレスを含むリクエストが届きます。私たちを経由するものはありません。
- AI の機能が使うのは、Apple の端末内のモデルだけです。Private Cloud Compute は使いません。
- 分析の SDK、クラッシュ報告の SDK、広告は入っておらず、トラッキングもしません。
- アプリからあなたの情報が私たちに届くことはありません。例外は 2 つです。ご自分でフォームから送ったお便りと、Apple が開発者に渡す報告です（「お問い合わせについて」「Apple から届くもの」を参照）。

### iPhone の中に置くもの

アプリは、iPhone 上のアプリ専用の置き場に次のものを保存します。

- 保存したリンク（届いたままの形）
- リンクごとに取得したもの: 題、説明文（X の投稿なら本文）、サイト名、著者、公開日、読む時間の目安、プレビューの絵 1 枚、サイトのアイコン
- ご自分で作ったもの: ポーチ（フォルダ）、リンクに付けた名前、メモ、ポーチの印（印に選んだ写真を含む）
- 端末内 AI が作った概要
- アプリの設定と、For you の動作に必要な記録。今日出したリンク、この先の数日ぶんの予定、「傾向でおすすめ」がオンなら最近のリンクから読んだ話題と、各リンクがその話題にどれだけ近いかです

記事の本文は、読む時間の目安と概要を作るために読みます。読んだ本文はメモリの中に置くだけで、リンクと一緒には保存しません。

共有シートから保存したときは、ページの先頭（256 KB まで）とプレビューの絵を、アプリと共有拡張が一緒に使う置き場に一時的に置くことがあります。次にアプリを開いたときに使い、使い終わったら消します。残ったものも 24 時間で消えます。

iCloud バックアップやコンピュータで iPhone をバックアップしている場合、iOS はほとんどのアプリと同じように、このアプリのデータもバックアップに含めます。そのバックアップはお使いの方と Apple のあいだのもので、私たちからは見えません。

### いつ、どこへつなぐか

#### いつ

- リンクを保存したあと（共有シート、貼り付け、ショートカットのいずれでも）
- 共有した直後に、共有拡張がページとプレビューの絵を取りにいきます。アプリを開いたときにプレビューがそろっているよう、iOS のバックグラウンドのダウンロードに取得を頼むこともあります
- 保存した直後の取得に失敗したときは、数秒後に 1 回だけやり直します
- 「取り直す」を押したとき
- アプリを開いているあいだ、保存済みのリンクを 1 件ずつ読み直して、読む時間と概要のための本文を取ります。本文がもうメモリにないリンクの長い概要を作るときも、そのページをもう一度読みます

取得のきっかけはリンクの保存です。プレビューを取らずにリンクだけ保存する設定はありません。

#### どこへ

1. **保存したリンクのサイトと、そこから転送された先のサイト。** Apple の LinkPresentation を通してページを取りにいきます。Safari やメッセージがリンクのプレビューに使うのと同じ、iOS の標準機能です。アプリ自身もページの HTML を読みます。読むのは先頭 64 KB までで、記事かもしれないページだけ 1.5 MB まで読みます。
2. **そのページが、プレビューの絵とアイコンの置き場として指している先。** コンテンツ配信網など、別の会社のサーバーであることがよくあります。アイコンを指定していないページには、そのサイトの `/favicon.ico` を取りにいきます。
3. **YouTube と X（それぞれのリンクのときだけ）。** YouTube の動画リンクでは、YouTube 公式の埋め込みの窓口（`www.youtube.com/oembed`）に動画の題とチャンネルを尋ねます。X の投稿リンクでは、X 公式の埋め込みの窓口（`publish.x.com/oembed`）に投稿の本文・投稿者・日付を尋ねます。X への問い合わせには、X の追跡拒否の指定（`dnt=true`）を付けています。
4. **リンクを含む X の投稿のとき:** 行き先を知るために X の短縮 URL の窓口（`t.co`）につなぎ、そのあと行き先のサイトに 1・2 と同じようにつなぎます。

#### 相手に届くもの

- リンクのアドレス全体。含まれるパラメータもすべて届きます。3 の埋め込みの窓口には、リンクが問い合わせのアドレスの一部として届きます。
- IP アドレス。インターネットにつなぐときは、どの通信でも届くものです。
- 通信の標準のヘッダ。User-Agent にはリクエストを送るソフトウェアの名前が入り、リクエストによっては Linkpoche の名前も入ります。ページを取るリクエストには Accept-Language も付けます。iPhone に設定している言語の一覧で、相手がその言語で返せるようにするためのものです。

アカウント、識別子、メモ、ほかのリンクなど、保存したものは相手に届きません。アプリが送っていないからです。届いたリクエストを相手のサイトがどう扱うかは、そのサイトとそのサイトのプライバシーポリシーによります。ブラウザでリンクを開いたときと同じ種類のリクエストです。

リンクを開くと、アプリはそのリンクをブラウザか、そのリンクを扱うアプリに渡します。そこから先の通信はそのアプリが行います。

### 端末内 AI

Apple Intelligence が使えて、オンになっている iPhone（iOS 26 以降）では、Linkpoche はそれを使って短い概要と AI タブの長い概要を作り、新しいリンクの行き先のポーチを示し、最近の関心からおすすめを選びます。

- 使うのは Apple の Foundation Models の端末内のモデルだけで、Private Cloud Compute は使いません。AI の機能がリンクを外へ送ることはありません。
- モデルが読むもの: リンクの題・説明文・本文の先頭、ポーチの名前と各ポーチのリンクの題を数件、最近保存したリンクの題・サイト名・概要です。
- リンクが関心にどれだけ近いかは、Apple の NaturalLanguage で測ります。これも iPhone の中で動きます。
- 設定の「端末内 AI」にスイッチが 3 つあります（「概要を作る」「行き先を照らす」「傾向でおすすめ」）。どれも最初はオンです。「概要を作る」を切ると、新しい概要を作らず、作った概要も表示しなくなります。「傾向でおすすめ」を切ると、話題と近さの記録を iPhone から消します。

### ホーム画面のウィジェットと Spotlight

- **ウィジェット。** 「今日の再会」ウィジェットのために、アプリはこの先のおすすめの写しを、ウィジェットと一緒に使う置き場に書きます。写しに入るのは、リンクごとの題、サイトのホスト名、ポーチ名、保存した日付、小さな絵です。リンクのアドレス、メモ、説明文、AI の概要は入れません。ウィジェットの中身は、ホーム画面が見える人なら誰でも見られます。
- **Spotlight。** Linkpoche は保存したリンクを iOS の端末内検索に載せます。「最近削除した項目」のリンクは載せません。1 件に入るのは、題（なければホスト名）、ポーチ名、サイト名またはホスト名、著者、短い AI の概要（あれば）、小さな絵です。リンクのアドレスとメモは入れません。Apple によると、この検索用のデータは端末の中にとどまり、Apple には共有されず、ほかの端末とも同期されません。リンクを削除すると、Spotlight からも外れます。

### クリップボード

貼り付けの近道を出すため、アプリはクリップボードに「Web のリンクらしきものがあるか」だけを iOS に尋ねます。iOS は、クリップボードの中身をアプリに見せずにこれに答えます。中身を読むのは貼り付けを押したときだけで、そのとき iOS が許可を求めます。ショートカットのアクションはショートカットからリンクを受け取るので、アプリ自身はクリップボードに触れません。

### 書き出しと取り込み

- 書き出しは、リンクと一緒に保存しているものすべて（メモと概要を含む）、ポーチ、絵を zip にまとめ、共有シートを開きます。行き先はご自分で選びます。控えは、次に書き出して置き換わるか、iOS が一時ファイルを片付けるまで、アプリの一時フォルダに残ります。
- 取り込みは、ご自分で選んだ zip を読みます。読み終えたら、アプリが持っている複製を消します。

### 削除

- 削除したリンクは、絵を持ったまま「最近削除した項目」に移ります。「最近削除した項目」には 50 件まで入り、51 件目が入ると、いちばん古いものを完全に削除します。「すべて完全に削除」を押すと、その場で空になります。
- 設定の「保存した画像をすべて消す」を押すと、リンクは残したまま、保存した絵とアイコンをすべて消します。
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

### このポリシーの変更

変更したときは、新しい日付を付けてこのページに載せ、同じリリースで App Store の掲載情報も更新します。黙ってアップデートし、データを集め始めることはしません。

### 連絡先

ご意見フォーム: https://forms.gle/GqJSQ4cF1YpSt5vx5
