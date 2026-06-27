# EasyCan — public showcase

> **Buy a canister, not a subscription.**

Source for the EasyCan landing page, served by GitHub Pages at
**<https://icp-easycan.github.io>**.

[EasyCan](https://icp-easycan.github.io) is a marketplace for apps that run entirely
on-chain on the [Internet Computer](https://internetcomputer.org) — each one inside a
*canister* (a smart contract) that **you** own. No accounts to lock you in, no servers
to trust, no vendor that can switch you off.

## What makes it different

- **Sovereign after claim** — when you take an app, you take its canister and become its
  only controller. From that moment EasyCan holds no keys to it: no backdoor, no admin
  recovery.
- **Verifiable from source** — every release is a reproducible build. The hash you can
  rebuild from the public source matches the code actually running on-chain, byte for byte.
- **No lock-in, ever** — your app keeps running as long as its canister has fuel, whether
  or not EasyCan still exists. Bookmark it and open it directly.

## The apps

- **Messenger** — private, on-chain messaging.
- **Vault** — end-to-end encrypted file storage.

More to come. Tap a card on the [site](https://icp-easycan.github.io/#apps) to see what
each one does, in plain language.

## Opening a Time Capsule

A Time Capsule is a sealed message or file an EasyHub user can leave to be delivered later
— to an heir, or to their future self. If one was delivered to you, open it here:

**<https://icp-easycan.github.io/open>**

The opener is a single, self-contained HTML page that runs **entirely in your browser** —
no network requests, no accounts. Paste the sealed capsule and the passphrase you were given
separately, and it reconstructs the message or file locally. For peace of mind, disconnect
from the internet first.

**Verifying the opener.** A tampered opener could steal your passphrase, so the page is
published with its SHA-256 at [`/open/SHA256.txt`](https://icp-easycan.github.io/open/SHA256.txt).
Save the page, run `sha256sum` on it, and confirm it matches. The strongest check is to
compare that value against this repository's git history, where any change would be visible.

---

> ℹ️ This repository is a **generated artifact**. The page source lives in a private
> monorepo (`site/`) and is published here by a script — do not edit these files by hand,
> changes would be overwritten on the next publish.
