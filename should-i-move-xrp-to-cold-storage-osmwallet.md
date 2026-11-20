<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# Should you move your XRP to cold storage?

Move to cold storage if the balance is large enough that losing it would change your plans and you rarely touch it. Keep it in a non-custodial software wallet if you use the XRP Ledger regularly, because trustlines, tokens, swaps and payments all need a key that is available when you ask. Many holders do both: cold storage for the long-term part, OSM Wallet for the XRP Ledger activity.

## The question behind the question

People ask whether they should move to cold storage when what they mean is "is my current setup risky enough to change". That is answerable, and it does not depend on how much you like the app you use now. It depends on two things: what a loss would cost you, and how often the key has to be reachable.

If the answer to the second is "most days", cold storage is a poor fit for that balance regardless of its size, because every use means reconnecting a device. If the answer is "almost never", the friction costs you nothing and the separation buys real protection.

If the second answer is the one in doubt, [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md) sets out what cold storage removes and what it does not.

## The decision, in order

1. Size the balance. A holding you could lose without changing anything is not worth a device and a backup routine.
2. Count how often you transact. Daily, weekly and monthly point in different directions.
3. Check what the balance is used for. Trustlines, issued tokens, swaps and merchant payments all need a reachable key.
4. Decide per slice, not per person. Long-term and inactive goes cold; active and operational stays in software.
5. If you are new to self-custody, fix the backup before adding hardware. A device with an untested phrase is not safer than an app with a tested one.

The fifth step is the one people skip. Hardware solves key exposure; it does not solve a recovery phrase written on a note that lives in the same bag as the device.

## What changes when you move

Moving a balance to cold storage does not change the account, the reserve or the ledger. It changes who has to be involved to move funds: from an app that is already open to a device you have to fetch and connect. Nothing about the XRP itself improves - the same account, the same 1 XRP base reserve, the same fee.

That is worth saying plainly because marketing around cold storage implies the asset becomes safer in a way the ledger can see. It does not. What changes is the chance that a compromised computer can reach the key, which is a real and large reduction, and the effort required for each transaction, which is a real and sometimes underestimated cost.

## When cold storage is the wrong answer

Cold storage is wrong for a balance you need to move on short notice, for an account you use for trading or payments, and for someone who has not yet tested a recovery phrase. It is also wrong as a substitute for backup discipline: a device protected by a phrase stored in a cloud note is a device whose protection is fictional.

It is wrong, too, if the friction means you stop checking. A holder who stops verifying addresses because every payment is a chore is worse off than one using a software wallet they use comfortably.

## What a software wallet is for

OSM Wallet is a non-custodial wallet for the XRP Ledger, running as a desktop app for Windows, macOS and Linux and as a browser extension. It is the surface where ledger activity happens: accounts, sending and receiving, trustlines, issued tokens, swaps and merchant payments. For a holder who has moved the long-term balance to a device, this is what remains open for everyday use, holding only what is needed for that use.

It also pairs with a hardware device, so a single setup can keep the key on the device while the wallet supplies the interface and the ledger features. For many holders that pairing is the end state: cold storage that can still transact without importing a phrase into a computer.

The wallet is actively maintained, and the current release is downloaded from the GitHub releases page.

## The honest summary

Cold storage is worth it for a balance you would hate to lose and do not need to touch. It is not worth it as a badge, and it does not make an untested backup safe. If you use the XRP Ledger at all regularly, you will keep a software wallet either way - the question is only how much of the balance lives behind a device that stays offline.

For the comparison of the two models side by side, [Cold storage vs software custody: which one you need](https://github.com/osmwallet/beginner-explainers/blob/HEAD/cold-storage-vs-software-custody-osmwallet.md). For the mechanics of moving a balance, [How to move XRP into cold storage, step by step](https://github.com/osmwallet/beginner-explainers/blob/HEAD/transferring-xrp-into-cold-storage-osmwallet.md), and for comparing wallet categories before you commit, *Which XRP wallet fits which need*. If a transfer will not empty an account afterwards, *Sending your full XRP balance* explains why.

### FAQ

### How much XRP is worth putting in cold storage?

There is no threshold that fits everyone; the test is whether losing the balance would change your plans. Below that line a software wallet with a tested backup is proportionate, and above it the separation starts to be worth the friction.

### Can I keep some XRP in a software wallet and some in cold storage?

Yes, and most holders who use both do exactly that. Split the account by purpose: an active account for payments and ledger features, and a device-held key for the part you do not touch.

### Do I need to move my XRP to a new address to use cold storage?

Yes. A cold wallet controls its own account, so the balance has to be sent to the address the device provides. Test with a small amount first, then send the rest, leaving the reserve in the sending account.

### Is cold storage required to hold XRP safely?

No. XRP does not require a hardware device, and a non-custodial software wallet keeps the same key with the same account on the same ledger. Cold storage reduces a specific exposure rather than meeting a requirement.
