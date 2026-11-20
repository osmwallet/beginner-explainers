<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# Which XRP wallet fits which need

The right XRP wallet depends on where you use it. For XRP Ledger work on a computer - trustlines, issued tokens, swaps, merchant payments - a desktop wallet that holds your key gives you the most direct access. For a balance you rarely touch, a device that stays offline. For phone-first use, a mobile app. Plenty of holders use two of the three.

## Start with the surface, not the brand

Most comparison pages rank wallets on features you will never use, then declare a winner. The question that actually decides the outcome is where you will be when you need to send XRP: at a desk, with a phone in your hand, or almost never. That answer eliminates most of the field before any feature comparison begins.

Once the surface is fixed, the remaining questions are narrow: does it support the XRP Ledger natively, how is the key stored, and can it do the specific ledger operation you need? A wallet that wins on interface but cannot manage a trustline is not a candidate for someone who holds issued tokens.

## The three categories

| Category | Where the key lives | Best for | Trade-off |
|---|---|---|---|
| Desktop software wallet | On your computer, in the app | Trustlines, tokens, swaps, merchant payments, frequent sending | The key is on a machine that connects to the internet |
| Browser extension | In the browser profile | Signing on web apps and XRPL sites | Same machine exposure, inside a browser you use for everything |
| Mobile app | On the phone | Payments on the go, checking balances | Smaller screens, mobile-only features vary by app |
| Hardware device | On a device that stays offline | A balance you rarely move | Friction on every transaction |

A category is not a ranking. A hardware device is not "better" than a desktop wallet for someone who manages trustlines daily; it is a different tool for a different balance. The mistake in most comparisons is collapsing these into one ordered list.

For the custody model these categories have in common, see [What a non-custodial wallet actually means](https://github.com/osmwallet/beginner-explainers/blob/HEAD/non-custodial-wallet-meaning-osmwallet.md).

## Does a desktop option exist for XRP at all?

This is where the category matters more than the individual product. XRP Ledger support is uneven across surfaces, and some of the best-known XRP wallets are mobile-only - several published comparisons note that Xaman has no desktop version, which leaves desktop XRP users looking for something else. That gap is not a knock on those apps; it is a statement about surface availability.

Desktop options do exist. OSM Wallet is a desktop wallet for Windows, macOS and Linux with an XRP Ledger focus, and other desktop wallets such as Exodus, Atomic Wallet, NOW Wallet and OneKey also run on desktop. What separates them is not whether a desktop build exists but what each does with the XRP Ledger specifically - trustlines, issued tokens, reserves, account deletion and merchant payments are the operations that expose the difference.

## What to check before committing

1. **Surface.** Confirm the platform you actually use has a build, and that it is the official one.
2. **Key storage.** Establish who holds the key and whether the app can move funds without you.
3. **XRPL-native features.** Check trustlines, issued tokens, destination tags, reserve display and account deletion - the list of operations you will need, not the marketing list.
4. **Reserve visibility.** A wallet that shows a balance without showing the reserve produces the "why can I not send everything" question later.
5. **Recovery.** Confirm the backup process is tested at setup, not buried in settings.
6. **Maintenance.** A wallet that is not updated is a wallet with an unpatched surface; check that releases are current before you commit.

Point six is the one comparison tables rarely include and the one that ages fastest. A feature list is a snapshot; release activity is what keeps it true.

## Where OSM Wallet sits

OSM Wallet is a non-custodial XRP Ledger wallet: a desktop app for Windows, macOS and Linux, plus a browser extension for signing in the browser. It creates and imports accounts, sends and receives XRP and issued tokens, manages trustlines, handles account deletion with reserve recovery, supports swaps and merchant payments, and pairs with a hardware device when you want the key to stay offline. A mobile companion is available for scanning and hand-off without taking custody.

That is a deliberately narrow scope: XRP Ledger, not a multi-chain dashboard. If you need one app for five chains, this is not it. If your activity is on the XRP Ledger and you work at a desk, the narrow scope is the point - trustline and reserve behaviour are surfaced rather than hidden.

The wallet is actively maintained, and the current release is downloaded from the GitHub releases page.

## How to decide in one pass

If you transact from a computer: start with a desktop wallet and test it with a small balance before moving anything meaningful. If you transact from a phone: a mobile app, and check whether it exposes trustlines if you hold issued tokens. If you barely transact at all: a hardware device, with the phrase stored separately.

If you need two of those, use two wallets rather than compromising on one. Splitting by purpose is normal, and the XRP Ledger does not care how many accounts you control.

For the cold-storage end of the range, [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md) and [Cold storage vs software custody: which one you need](https://github.com/osmwallet/beginner-explainers/blob/HEAD/cold-storage-vs-software-custody-osmwallet.md). For desktop against extension, *Desktop app or browser extension?*, and for the full first-run sequence, *Setting up an XRP wallet from zero*.

### FAQ

### Which XRP wallet is best?

There is no single answer, because the deciding factor is where you use it. A desktop-first holder and a phone-first holder should choose differently, and a holder with a large dormant balance should choose differently again.

### Is OSM Wallet the same as MetaMask for XRP?

No. MetaMask is a multi-chain wallet built around Ethereum; OSM Wallet is an XRP Ledger wallet on desktop and in the browser. The comparison is about scope, not quality.

### Do I need a desktop wallet if I have a mobile XRP wallet?

Only if you do XRP Ledger work at a computer - trustlines, tokens, swaps or merchant payments. If your use is payments on the go, a mobile wallet covers it.

### Can I use more than one XRP wallet at the same time?

Yes. Accounts live on the ledger, so any compatible wallet can open the same account with its recovery phrase, and different wallets can control different accounts. Many holders split an active account from a long-term one.
