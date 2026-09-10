---
layout: default
title: Exif Off Support
---

# Exif Off Support

Exif Off removes location, capture date, and device metadata from copies of your photos, entirely on your iPhone.

## Contact

Support form: https://docs.google.com/forms/d/e/1FAIpQLSeXsM3xUSTul95Di11zZ08k39UTBjzMGTJu83BS0-8Gm2ukIw/viewform

The form asks for three things: your email address, a subject, and your message. There is no sign-in and no account. Your address is used to reply to you and for nothing else.

One person reads what comes in, and every message that arrives gets a reply. There is no promised turnaround here: a number of days is a promise one person cannot keep in every week of the year, so it is not made. What you do get is an answer from the person who wrote the app, and no message goes unanswered.

If a week goes by with no reply, send the form again, and check the address you typed while you are there. A typo in it leaves no way for a reply to reach you.

Most of what people write in about is answered below already, and those answers do not have to wait for anyone.

The form has no attachment field, so everything has to go in the message. Useful to include:

- Your iPhone model and iOS version.
- The version of Exif Off, from the Version row on the Settings screen in the app.
- The file type involved: JPEG, PNG, or HEIC.
- Which action you used: "Remove location only" or "Remove all metadata".
- What you saw, and what you expected instead.

Please do not send us the photo itself. We do not need it to answer most questions, and a photo you are worried about is the last thing you should be sending to anyone.

## Frequently asked questions

### How do I check that the metadata is really gone?

Run the cleaned copy back through Exif Off. Select it, open its detail screen, and read the list. Removed fields are not shown at all, so a fully cleaned photo shows almost nothing.

As a second check, open the copy in the Photos app and tap the info button. A photo that still carries coordinates shows a map there. A cleaned copy does not.

### What happens to my original photo?

Nothing. Exif Off never edits the original. It reads the file, writes a new copy with the metadata removed, and saves that copy as a new photo in your library. Afterwards you have both, and you decide which one to keep and which to delete.

This is also why the copy is the one to share. If you share the original by mistake, the original still carries everything it had.

### Which formats are supported?

JPEG, PNG, and HEIC.

The image itself is never re-encoded. Only the metadata sections of the file are rewritten, so a HEIC photo stays a HEIC photo at its original quality and the picture is identical to what you started with.

Live Photos, video, and RAW files are not supported in this release.

### Why did one photo fail when the rest went through?

A small number of HEIC files keep their metadata in a layout that cannot be rewritten without re-encoding the image. Exif Off will not quietly degrade a photo, so it skips that file, reports it as skipped, and finishes the rest of the batch. The skipped file is left exactly as it was.

If you need that particular photo cleaned, make a JPEG copy of it with any app that exports JPEG and run the JPEG through Exif Off. Be aware that converting to JPEG re-encodes the image, so the quality does change.

It also helps to send us the iOS version and the camera or app that produced the file. Layouts we can handle without re-encoding are worth adding.

### I only removed the location, so why did my caption and keywords disappear?

"Remove location only" also drops three blocks: XMP, IPTC, and MakerNote. Each of them can hold coordinates of its own, and there is no way to lift only the location out and leave the rest intact, so they are removed whole. Captions, keywords, titles, and similar notes live in those same blocks.

Your original still has all of it. If those notes matter more to you than the location does, keep the original and share that instead.

### The cleaned copy still shows a date in the Photos app. Did it not work?

The Photos app keeps its own record of each item in your library, including when it was added, and it shows that record in its own interface. That record sits in your library on your device.

The file is the part you send to other people, and in the cleaned copy the file has no capture date left in it. To see what the file contains rather than what your library remembers, run the copy back through Exif Off and read the detail screen.

### There is still a thumbnail inside the file. Why?

Because you used "Remove location only". The Exif preview thumbnail is stored inside the Exif block, and that mode rewrites the block rather than removing it: the coordinates come out and the thumbnail stays.

"Remove all metadata" takes the whole Exif block out, and the thumbnail goes with it.

So if the thumbnail is the part you are worried about, use "Remove all metadata". That is worth doing for a photo you have cropped or edited, because an Exif thumbnail is not always regenerated after an edit and can still show the earlier version of the picture.

### Can I process more than 20 photos at once?

Not in this release. Twenty photos per run is the limit and it is shown on screen. Run it again for the next twenty.

### Does the app send anything anywhere?

No. Exif Off makes no network requests at all. There is no networking code in the app, and no server of ours for anything to go to. There is no account, no advertising, and no analytics or crash reporting SDK in it.

One thing in the app can lead to the internet, and it is worth being exact about: the Settings screen has two links, one to the support form and one to the privacy policy. Tapping one hands the address to your browser, and your browser loads the page. The app does not fetch anything itself, and nothing about you is added to the link.

The privacy policy at https://da-takatsuki.github.io/apps-pages/exif-off/privacy-policy.html lists what is not collected, item by item.

### Can it edit metadata, or put a different date or location on a photo?

No. Exif Off only removes. There is no way to add or change a field.

### Why is the cleaned copy a slightly different size?

The metadata is gone, so the file is a little smaller. The image data is unchanged.

### The app is not doing what I expected. Can I get a refund?

If something is not working the way the App Store description said it would, send a message through the support form and say what happened. Much of what comes in turns out to be a file this release does not handle, or the difference between the two removal modes, and either can be settled in one reply. If it is a bug, we would rather fix it than keep the money for something broken.

If you would rather have the money back, that request goes to Apple.

Apple is the seller of every app on the App Store. Apple takes the payment and Apple decides refunds. We never see your purchase, your payment method, or your Apple Account, so there is nothing on our side to press, and we cannot check on a request you have already filed.

To ask Apple:

1. Go to reportaproblem.apple.com and sign in with the Apple Account you used to buy the app.
2. Choose "Request a refund".
3. Choose the reason, then select Exif Off from your list of purchases.
4. Submit the request.

Apple asks you to allow 24 to 48 hours for an update on the request, and if it is approved the money can take longer than that to reach your payment method. Apple's own instructions, including the other ways to reach the same form, are at https://support.apple.com/en-us/118223

Eligibility is Apple's decision and depends on where you live, under the Apple Media Services Terms and Conditions. Nothing here limits the rights you have under the consumer law where you live, and Apple notes that customers in Australia and New Zealand keep their statutory rights in particular.

## Known limits in this release

- Up to 20 photos per run.
- The picker shows your 300 most recent photos. There is no album view, search, or "load more" yet, so photos older than that cannot be reached in this release.
- JPEG, PNG, and HEIC only. Videos cannot be selected at all, a RAW file is reported as skipped, and a Live Photo is read as its still image, so the copy Exif Off saves is a still photo.
- Originals in your Photos library are never modified. A cleaned copy is saved instead.
- "Remove location only" also removes XMP, IPTC, and MakerNote, and with them any captions or keywords stored there.
- The ICC color profile is kept, even under "Remove all metadata", so colors do not shift.
- The Exif preview thumbnail is kept under "Remove location only" and removed under "Remove all metadata", which takes out the whole Exif block.
- Some unusual HEIC files are skipped rather than re-encoded.
- Available in English and Japanese. The app follows your device language.

## Links

- Privacy policy: https://da-takatsuki.github.io/apps-pages/exif-off/privacy-policy.html
- Support form: https://docs.google.com/forms/d/e/1FAIpQLSeXsM3xUSTul95Di11zZ08k39UTBjzMGTJu83BS0-8Gm2ukIw/viewform
