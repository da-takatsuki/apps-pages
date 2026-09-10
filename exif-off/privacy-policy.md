---
layout: default
title: Exif Off Privacy Policy
---

# Exif Off Privacy Policy

Last updated: 2026-09-11

Exif Off does not collect any data. Not for analytics, not for advertising, not in anonymized form, not in aggregate. The rest of this page is that same answer, item by item, because a sentence about caring is not information.

Exif Off is published by Daiki Takatsuki. Contact: the support form at https://docs.google.com/forms/d/e/1FAIpQLSeXsM3xUSTul95Di11zZ08k39UTBjzMGTJu83BS0-8Gm2ukIw/viewform

## The short version

- The app reads the photos you select and writes cleaned copies. Both stay on your device.
- The app makes no network requests. There is no networking code in it, and no server of ours for anything to reach.
- No account, no sign-in, and no identifier of any kind.
- No analytics SDK, no crash reporting, and no advertising.
- The app tells us nothing about you, so there is nothing for us to keep, lose, sell, or hand over. The one exception is a message you choose to send us through the support form. See "If you contact us".

## What the app does with your photos

When you select photos, Exif Off reads them from your photo library to show you what metadata they contain and, if you ask it to, to write a copy with that metadata removed.

- Photos and their metadata are read into memory on your device. They are not transmitted anywhere.
- Cleaned copies are saved back to your photo library as new photos. The originals are left unchanged.
- When you send a cleaned photo on through the share sheet, a copy is written to a temporary folder so that the receiving app can read it, and that folder is deleted as soon as the share sheet closes. Nothing else is written outside your photo library.
- Nothing about a photo is kept by the app afterwards. No list of the files you processed, no history, and no stored copy of the metadata it showed you.

iOS asks for your permission before the app can see your photo library. That access is used only for the above, and you can revoke it at any time in the Settings app.

## Data we do not collect

We do not collect, receive, store, sell, share, or otherwise process any of the following:

- Your photos, or copies of them.
- The metadata read from your photos, including GPS coordinates, capture dates, camera and lens names, and any captions or keywords.
- Your name, postal address, or date of birth.
- Your email address, except the one you type into the support form yourself. See "If you contact us" below.
- Your phone number.
- Your location, at any precision, from any source.
- Device identifiers, including the advertising identifier (IDFA), the vendor identifier (IDFV), the device name, and the serial number.
- Your IP address.
- Your Apple Account, or any other account. There is no account in this app.
- Usage and product interaction data: which screens you opened, which buttons you tapped, which features you used, how long you used the app, or how many photos you processed.
- Performance data: crashes, hangs, or energy use.
- Diagnostics or logs of any kind sent off your device.
- Search history, browsing history, or the contents of any other app.
- Contacts, calendars, health data, fitness data, financial data, or purchase history.
- Advertising identifiers, cookies, tracking pixels, or device fingerprinting signals.
- Any of the above in anonymized, hashed, or aggregated form.

## No third parties

Exif Off contains no analytics, attribution, advertising, crash reporting, or A/B testing SDK. There is no advertising in the app, and no data is used for tracking as Apple defines it.

It is built with open-source Flutter packages, which is ordinary for an iOS app: they read your photo library, show the system share sheet, open links in your browser, and parse image metadata. None of them is an analytics or advertising component, and none of them is given a photo to send anywhere.

## No network

The app makes no network requests. There is no backend service, no telemetry endpoint, and no remote configuration, and there is no Exif Off server anywhere. This is a property of the code rather than a promise about our conduct: there is nothing in the app that can open a network connection.

We checked that instead of assuming it, and we checked the app we actually ship. None of the binaries inside it link against Apple's networking frameworks, and the compiled Dart code contains no HTTP client at all. Some of the open-source packages Exif Off is built on do carry network code for other platforms, in a web or Android build path; none of it reaches the iPhone app. A test in our build fails if a package that can reach the network is ever added, so this stays true release to release.

One thing in the app leads to the internet, and it is worth being exact about: the Settings screen has two links, one to the support form and one to this policy. Tapping one hands the address to your browser, and your browser loads the page. The app does not fetch anything itself, and nothing about you is added to the link.

## If you contact us

The support form is the only route by which we receive anything from you, and we receive only what you type into it.

- The form asks for three things and nothing else: your email address, a subject, and your message. There is no attachment field.
- It is a Google Form, hosted by Google. What you type is sent to Google's servers and stored there, in our Google account, which is where we read it. Google is handling it in order to deliver it to us, the same position an email provider would be in. What Google does as the host of that page is covered by Google's own privacy policy at https://policies.google.com/privacy
- The form does not ask you to sign in, and it is not set to collect the Google account of whoever fills it in. The only address that reaches us is the one you type.
- We use your address to reply to you, and for nothing else.
- We do not add you to a mailing list.
- We do not share what you send with anyone else.
- We delete support messages once they are resolved and no longer useful for handling a repeat of the same problem.
- Please do not send us a photo. We do not need one to answer most questions.

## What Apple tells us

Apple gives every developer sales and download reports for their own app: counts by country and by date. They do not identify anyone, and we never learn who downloaded Exif Off. That is Apple's reporting to a developer, not data collected by the app, and it is the only thing that ever reaches us about anyone using it.

## Children

The app collects nothing from anyone, at any age.

## Your rights

Requests to access, correct, delete, or export your data all have the same answer: the app tells us nothing about you, so there is nothing from it to access, correct, delete, or export. The one thing we can hold is a message you sent through the support form, along with the address you typed into it, and if you ask us to delete that we will.

## Changes to this policy

If this ever changes, the new version will be posted here with a new date at the top, and the App Store listing will be updated in the same release. We will not begin collecting data in a silent update.

## Contact

Support form: https://docs.google.com/forms/d/e/1FAIpQLSeXsM3xUSTul95Di11zZ08k39UTBjzMGTJu83BS0-8Gm2ukIw/viewform

## Links

- Support: https://da-takatsuki.github.io/apps-pages/exif-off/support.html
