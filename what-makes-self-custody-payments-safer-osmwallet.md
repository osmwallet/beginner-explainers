<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# What makes self-custody payments safer

A self-custody payment goes from your wallet straight to the XRP Ledger, so no company sits between your approval and the transaction. You see the destination, the amount and the fee before anything is submitted, and nobody can block, reorder or cancel it afterwards. What makes it safer is also what makes it unforgiving: the address you confirm is the address that gets paid.

## What is different about paying from your own wallet

The difference is who executes. A custodial service moves an internal number and settles with the ledger on its own schedule; a self-custody wallet submits your signed payment to the ledger directly. That removes a queue, a withdrawal limit and an operator who can decide your transaction is not happening today, and it also removes the person who could have caught your typo.

Speed is the visible part. The invisible part is the record: the ledger credits the payment to your account, and the receiving account's balance changes once the transaction validates. There is no intermediate state where a company owes you money.

## What you approve, and what the wallet does

The wallet's job is to show you the transaction accurately and submit exactly that. Everything else - trusting the destination, reading the tag, choosing an amount - is yours, which is why the confirmation screen deserves more than a glance.

| What you see | What it means | Who is responsible |
|---|---|---|
| Destination address | The account that will receive the XRP | You - check the first and last characters |
| Destination tag | A number some services need to credit the right customer | You - copy it from the receiving service |
| Amount | What leaves your account | You |
| Fee | The small ledger fee for the transaction | The wallet shows it, the ledger sets the floor |
| Remaining balance | What stays, including the 1 XRP base reserve | You - the reserve is not spendable |

The reserve row surprises people. An XRP Ledger account must hold a base reserve, so a payment that would empty the account is rejected rather than partially sent. That is a ledger rule, not a wallet preference, and it is the most common reason a transfer "will not go through".

## Where self-custody payments go wrong

Almost every failure is a destination problem rather than a wallet problem: an address copied from the wrong place, a missing tag for an exchange deposit, a token sent to an account that has no trustline for it, or a payment made on the wrong network. None of these are recoverable by the sender, and none are caused by the wallet holding the key.

The countermeasures are boring and effective. Paste rather than type, compare the first four and last four characters on both screens, send a small test amount to any new destination, and save the destination as a bookmark after the first success so a later payment cannot drift.

## The steps that make a payment safe

1. Confirm the receiving address on the device or screen the receiver controls, not from a chat message.
2. Enter the destination, then read the address back against the source.
3. Add the destination tag if the receiver is a service that issued one.
4. Check the fee and the amount that will remain, remembering the reserve.
5. Send a small test amount for a new destination and wait for it to validate.
6. Send the balance, then confirm the arrival before repeating the payment anywhere else.

Steps one and five prevent nearly every loss people report. The rest of the list exists because a payment that validates cannot be reversed by anyone, including the developers of the wallet.

## How OSM Wallet handles a payment

OSM Wallet runs on the XRP Ledger only, as a desktop app and a browser extension, and it holds your keys rather than holding your funds. You enter a destination, and the wallet shows the transaction for approval before submitting it; if a payment would leave too little for the reserve, it is rejected at the ledger. Destination tags and memos are supported for payments that need them, and the wallet can verify an incoming payment so you know the ledger accepted it.

When a payment does not go through, the cause is usually the reserve, a trustline that does not exist yet, or an amount that exceeds what is actually available. Those cases are covered in [Sending your full XRP balance](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/send-max-xrp-balance-osmwallet.md) and [Destination tags and memos, without the mistakes](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/destination-tags-and-memos-in-osmwallet.md), which is where most people land after their first failed send.

The wallet is actively maintained and the current release is downloaded from the GitHub releases page, so an update is the first thing to check when a payment behaves differently from this description.

## What self-custody payments do not protect

Self-custody does not stop you from approving a bad destination, and it does not make a phishing page safe. If a site asks you to type your recovery phrase to "verify" a payment, it is not verifying anything - the phrase is the account, and handing it over hands over the balance. Nor does it protect a machine that is already compromised: a wallet on an infected computer is a wallet whose confirmation screen cannot be trusted.

For the storage model that removes a device from the equation entirely, see [What is a cold wallet for XRP?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/what-is-a-cold-wallet-for-xrp-osmwallet.md). For the attacks that actually target XRP holders, see *How XRP gets stolen, and what stops it*.

## Where to go next

If you are still deciding who should hold your keys, start with *What a non-custodial wallet actually means*. If you want the ledger mechanics behind a balance and a reserve, read *How an XRP wallet holds your funds*. For a full balance transfer, *Sending your full XRP balance* covers the reserve arithmetic.

### FAQ

### Why is my payment rejected when I have enough XRP?

Because the base reserve must remain in the account. A payment that would drop the balance below the reserve is refused by the ledger, not the wallet. Reduce the amount, or check which funds are tied up in unfunded trustlines.

### Can a self-custody payment be reversed?

No. Once a transaction validates on the XRP Ledger it is final. That is the property that makes a self-custody payment reliable, and the reason a test payment to a new destination is worth the extra minute.

### Do I have to add a destination tag?

Only if the receiver requires one. Exchanges and services use tags to identify which customer a deposit belongs to; a personal wallet usually does not need one. Sending to a service without its tag can leave the deposit uncredited, so copy the tag from the service rather than guessing.

### Is a self-custody payment anonymous?

No. The XRP Ledger is public: addresses, amounts and timestamps are visible to anyone. Self-custody changes who controls the account, not who can read it, so treat every address you use as linkable.
