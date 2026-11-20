<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# How to move XRP into cold storage, step by step

Send XRP from your software wallet to the address your cold wallet provides, after confirming that address on the device's own screen. Start with a small test amount, confirm it arrives, then send the rest and leave the reserve behind. OSM Wallet handles the sending side of that: you enter the destination, check the amount and fee, and approve the payment.

## Before you send anything

Two things need to be true before the first payment. The cold wallet must already be set up with its recovery phrase written down and tested, and the address it gives you must be read from the device rather than copied from a chat, screenshot or email. A payment to a cold wallet is final like any other, and an address that came from the wrong place sends your XRP somewhere you do not control.

Also decide what stays behind. The sending account must keep its base reserve, and it needs a small amount for the transaction fee, so "send everything" is not an option the ledger offers. Work out the maximum you can send before you start, or the last transaction will fail after the earlier ones succeeded.

## The steps

1. **Open the cold wallet and get its receive address.** Use the device's own interface, not a saved note.
2. **Read the address on the device screen.** Compare the first four and last four characters against what the app shows. Malware can change a clipboard; it cannot change a device screen.
3. **Enter that address in OSM Wallet's send screen.** Paste it, then read it back once more against the device.
4. **Check the tag field.** A personal cold wallet usually needs no destination tag; if the device's interface shows one, use it. Never invent one.
5. **Send a small test amount.** A trivial sum confirms the address is correct and that the account is ready to receive.
6. **Confirm the test arrived** by checking the balance on the device, not only in the sending app.
7. **Send the rest**, leaving enough for the base reserve and the fee.
8. **Record what you did.** Note the date and the amount outside the wallet, so a later discrepancy is recognisable rather than mysterious.

Steps five and six are the ones that turn a mistake into a few dollars rather than a total loss. They cost a fee and a minute, and they are the entire difference between a careful transfer and a reported loss.

## How much to leave behind

The sending account needs its base reserve plus the fee, and any extra reserve it holds for trustlines. If the account holds issued tokens with trustlines, deleting it later releases that reserve but requires the trustlines to be removed first, which is a separate operation.

A simple rule: send the balance minus the reserve, minus a small margin for the fee. If the app refuses an amount, the amount is above what the ledger considers spendable rather than a fault - the arithmetic and the fix are in [Sending your full XRP balance](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/send-max-xrp-balance-osmwallet.md).

## What can go wrong, and what it looks like

| Symptom | Cause | What to do |
|---|---|---|
| The send is refused before submitting | Amount above the spendable balance once the reserve is counted | Reduce the amount, leave the reserve |
| The test payment never arrives | Address typed or pasted incorrectly, or the wrong network | Do not resend; re-read the address on the device |
| The balance shows nothing on the cold wallet | Device not synced to the right account, or the address belongs to another account | Check the receive address again against the sending history |
| Tokens moved but XRP did not | Issued tokens need a trustline on the receiving account | That is a separate operation; see [Issued tokens and TrustLines in practice](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/issued-tokens-and-trustlines-in-osmwallet.md) |

The fourth row is a common surprise: an XRP payment alone does not bring tokens, and a token transfer to an account without a trustline will not appear as a balance.

## How OSM Wallet handles the sending side

OSM Wallet is a non-custodial wallet for the XRP Ledger, available as a desktop app and a browser extension. It sends XRP and issued tokens, shows the destination, amount and fee before you approve, supports destination tags and memos where a receiver needs them, and verifies that an incoming payment was accepted by the ledger. It does not hold your keys, so it cannot and will not move anything without your approval.

The wallet is actively maintained, and the current release is downloaded from the GitHub releases page. If a send behaves differently from this description, updating is the first step.

## After the balance is moved

Keep the software account funded with enough for future activity, and keep the cold wallet's recovery phrase separate from the device. A cold wallet whose phrase is stored beside it is protected against malware and not against a house move, a fire or a bag left on a train.

For the decision to move at all, see [Should you move your XRP to cold storage?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/should-i-move-xrp-to-cold-storage-osmwallet.md) and *Cold storage vs software custody: which one you need*. For what the destination device does and does not protect, *What is a cold wallet for XRP?*. For tag rules on the receiving side, *Destination tags and memos, without the mistakes*, and for the reserve arithmetic, *The XRP reserve, explained without the confusion*.

### FAQ

### How much should I send first?

A small amount whose loss would not matter - enough to confirm the address and the account, not enough to hurt. Send the balance only after that test has arrived and been confirmed on the receiving device.

### Can I send XRP directly from an exchange to a cold wallet?

Usually yes, and the exchange withdrawal form is the same as any other. The difference is that you should still verify the address on the device before submitting it, because the exchange will not check it for you.

### Why does the wallet refuse to send my whole balance?

Because the account must keep its base reserve, and the transaction itself needs a fee. The spendable amount is the balance minus the reserve and fee; a payment above it cannot be valid.

### Do I need a destination tag to send to a cold wallet?

Normally no. Tags exist so services can credit the right customer; a personal hardware wallet's account is identified by its address alone. Use a tag only when the receiving interface shows one.
