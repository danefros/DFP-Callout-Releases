# DFP Callout — releases

This repository holds only two things:

- **`appcast.xml`** — the [Sparkle](https://sparkle-project.org) feed the app checks for updates. Signed with an EdDSA key held by DF Productions; the app verifies the signature before it will install anything.
- **Releases** — each build as a notarised, stapled zip, named `DFP-Callout-<version>-b<build>.zip`.

The app's source lives in a private repository. Nothing here is code.

## If you are a tester

You don't need this page. Callout checks this feed once a day and offers the update in the app; **Help → Check for Updates…** checks now. Turn automatic checks off in Settings → General if you'd rather.

What the app sends when it checks: one request for `appcast.xml`, carrying its own version number. Nothing about you or your Cards.

## Rolling back

Every build stays published. Download an older zip from the Releases page, quit Callout, and drag the app to Applications over the newer one. Your Library is untouched — it lives in your own folder, not inside the app.
