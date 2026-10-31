# Sidedrop

**AirDrop for people who use a Mac and an Android phone.** Over your own wifi. No cloud, no account, no Google servers.

- A menu-bar app on the Mac. Your phone shows up as a blue dot when it's nearby.
- "Sidedrop" in the Android Share menu. One tap, no app to install (it's a web page you add to the home screen).
- Drop a file anywhere on the Mac panel and it's on the phone.
- Files go straight from one device to the other, on your network.

**Landing page:** https://federicobuildz.github.io/sidedrop/ — leave your email to get one message when the proper version ships. No newsletter.

## Status

Personal tool, built in two evenings with [Claude Code](https://claude.com/claude-code). It runs every day on my Mac, but it's rough: a local certificate to install once on the phone, no pairing yet (anyone on your wifi could open the page).

The proper version, if there's interest: pairing, no manual certificate, starts at login. One-time price, around €9.99.

## Source

Not yet. Pairing first. This repository holds the landing page only.

## How it's built

- Mac: a SwiftUI menu-bar app compiled with `swiftc`, no Xcode.
- Server: ~300 lines of Node, HTTP and HTTPS.
- Android side: a web page with Web Share Target, served over HTTPS with a local CA so the Share menu accepts it.

Made in Rome by a window cleaner. Questions: open an issue.
