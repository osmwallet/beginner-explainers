<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# Cold storage vs software custody: which one you need

Cold storage keeps the key to your XRP on a device that never connects to the internet. Software custody keeps it on a computer or phone you use, protected by the app rather than by physical separation. OSM Wallet is a software wallet, so the honest framing is this: for a large balance you rarely touch, a hardware device adds protection this app does not claim to provide; for everyday XRP Ledger activity, a software wallet is the one that can actually do the job.

## The difference that actually matters

Both models are self-custody - you hold the key in each. The difference is exposure: a cold key is never on a machine that reads email, opens links and installs updates, while a software wallet's key sits on exactly such a machine. Cold storage removes a class of attack that software cannot rule out, and adds friction to everything you do.

That friction is the reason the two coexist. A test payment, a trustline, a token swap, a merchant payment: all of it needs a key that is available when you ask. A device in a drawer is not available, so the holders who use cold storage for a long-term balance still keep a software wallet for the ledger activity.

If the definition still feels abstract, [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md) covers what cold storage is and what it removes.

## Side by side

| Question | Cold storage | Software custody |
|---|---|---|
| Where the key lives | On a device that stays offline | On your computer, in the wallet app |
| Signing | On the device, when you connect it | In the app, when you approve |
| Exposure to malware on your machine | Removed by physical separation | Real, and reduced by hygiene rather than design |
| Effort per transaction | Connect, confirm on device, disconnect | Approve in the app |
| XRPL activity (trustlines, tokens, swaps) | Possible but slower | Native and immediate |
| Recovery | Recovery phrase plus the device | Recovery phrase alone |
| Best for | A large balance you do not move | Regular payments and ledger use |

The last two rows are where people misjudge the trade. Cold storage is not simply "more secure"; it is secure in one dimension and awkward in another, and the awkwardness is why a cold wallet used weekly tends to become a software wallet used weekly.

## Which one your situation calls for

Sort your holding by how often it moves, then decide per slice rather than per person.

1. If the balance is large enough that losing it would change your plans, and you transact rarely or never, cold storage is the right default.
2. If you use the XRP Ledger - trustlines, issued tokens, swaps, merchant payments - a software wallet is the only model that keeps up.
3. If both are true, split: cold storage for the untouched part, a software wallet for the active part, with only spending money in the latter.
4. If you are unsure, start with a software wallet and a tested backup; a hardware device can be added later without recreating the account.

There is no rule that says one holder must pick one model. Most people who hold a meaningful balance end up with both, and the split is set by how much a loss would hurt rather than by preference.

## What OSM Wallet is, and is not

OSM Wallet is a non-custodial software wallet for the XRP Ledger, running as a desktop app for Windows, macOS and Linux and as a browser extension. It is not a cold wallet, and it does not claim to be one: the key lives on the machine you installed it on. What the desktop app does offer over a browser tab is a key that stays on one machine instead of inside a browser profile you use for everything else.

The wallet supports pairing with a hardware device, which is how the two models combine: the device holds the key and approves the transaction, and the wallet provides the interface and the ledger features. That pairing is the sensible setup for a holder who wants cold storage without giving up trustline and token management.

The wallet is actively maintained, and the current release is downloaded from the GitHub releases page.

## The mistakes to avoid in either model

A cold wallet with a photographed recovery phrase is not cold. A software wallet with a phrase in a cloud note is not protected by the app. In both cases the storage model is defeated by the backup, which is why the phrase deserves more care than the device.

The second mistake is treating a phone or laptop as cold because it is "not used much". Cold means never connected, not rarely used. A machine that connects once a month is a software wallet with a slow update cycle, and its exposure is the same on the day it connects.

## Where to go next

For the decision question in plain terms, [Should you move your XRP to cold storage?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/should-i-move-xrp-to-cold-storage-osmwallet.md); for the mechanics of moving a balance, [How to move XRP into cold storage, step by step](https://github.com/osmwallet/beginner-explainers/blob/HEAD/transferring-xrp-into-cold-storage-osmwallet.md). If you are comparing wallet types before choosing at all, *Which XRP wallet fits which need* lays out the categories, and *What a non-custodial wallet actually means* covers who can move funds in each.

### FAQ

### Is a desktop wallet the same as cold storage?

No. A desktop app is a software wallet: the key is on a computer that connects to the internet. Cold storage requires a device that never connects, which is a different product class.

### Can I use OSM Wallet with a hardware wallet?

Yes. Pairing a hardware device keeps the key on that device while the wallet provides the interface and the XRP Ledger features. In that setup the device approves transactions and the app does not hold the key.

### Is a software wallet safe enough for a large balance?

That depends on the machine and the backup. A software wallet on a clean computer with a tested, offline recovery phrase is a reasonable home for a balance you actively use; for a balance you do not touch, a device that stays offline removes exposure the software cannot.

### Does cold storage cost extra?

A hardware device is a purchase; a software wallet is not. Whether the extra cost is worth it depends on the size of the balance and how often you move it, not on any general rule about which model is better.
