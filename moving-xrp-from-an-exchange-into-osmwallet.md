<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# Moving XRP from an exchange into your own wallet

Copy the receive address from OSM Wallet, paste it into the exchange's withdrawal form, and add the destination tag the exchange asks for - that tag belongs to the exchange, not to your wallet. Send a small amount first, confirm it arrives, then withdraw the rest. Once the payment validates, the account exists and must hold the 1 XRP base reserve.

## The two fields that decide whether the XRP arrives

Every exchange withdrawal form has an address field, and most have a second field for a tag or memo. Getting the first wrong sends the funds to an address nobody controls; getting the second wrong sends them to the exchange without telling it who they belong to. Both errors are final.

The address comes from your wallet: open the receive screen and copy it. The tag, if there is one, comes from the exchange - it identifies your account on their side, and it stays the same across withdrawals. A tag is not a property of your wallet, so never carry one over from a different service.

## The steps

1. **Open OSM Wallet and copy the receive address.** Read the first four and last four characters before you leave the screen.
2. **Open the exchange's XRP withdrawal form** and paste the address. Check the network selector says XRP Ledger, not another chain that also has XRP.
3. **Fill the tag field** only if the form shows one; copy the value from the exchange's own deposit instructions.
4. **Withdraw a small test amount** and wait for the exchange to process it.
5. **Confirm it arrived** in the wallet, and check the account now exists with its reserve.
6. **Withdraw the rest**, and keep the withdrawal record.

Exchanges batch withdrawals, so step four can take minutes to hours depending on the service. That waiting period is precisely why it belongs on the test payment rather than on the whole balance.

## What a tag is, and whose it is

A destination tag exists because one exchange address can serve thousands of customers. The address says which exchange, the tag says which customer. When you withdraw *to* an exchange, you supply their tag. When you deposit *from* an exchange into your own wallet, no tag is needed, because the address alone identifies you.

A wallet that asked for a tag when receiving would be unusual, and a form that requires a tag you do not have is a sign you are pasting into the wrong kind of destination. The rules and the exchange-side consequences are covered in [Destination tags and memos, without the mistakes](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/destination-tags-and-memos-in-osmwallet.md).

## What the account looks like afterwards

An XRP Ledger account that has never been funded does not exist yet, so the first payment both creates it and funds it. That first payment must cover the base reserve, which is why a withdrawal of a fraction of 1 XRP cannot activate an account on its own. After it exists, the reserve stays locked while the account does, and it is released when the account is deleted.

This is also the reason a withdrawal can arrive and still look short: the reserve is part of the balance but not spendable, so an account funded with exactly 1 XRP shows nothing available to send. The arithmetic is in [The XRP reserve, explained without the confusion](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/xrp-reserve-explained-osmwallet.md), and the activation sequence is in *Activating an XRP Ledger account*.

| Situation | What happens |
|---|---|
| First withdrawal, above the reserve | Account is created, balance shows the amount |
| First withdrawal, below the reserve | Withdrawal cannot activate a usable account |
| Withdrawal without the required tag | Exchange may not credit the deposit; contact them with the transaction ID |
| Withdrawal to an address you misread | Payment is final; nobody can reverse it |

## How OSM Wallet handles the receiving side

OSM Wallet is a non-custodial wallet for the XRP Ledger, on desktop for Windows, macOS and Linux and as a browser extension. It shows the receive address for the selected account, displays the balance the ledger reports including the reserve, supports destination tags and memos for payments that need them, and lets you verify that an incoming payment was accepted.

It is actively maintained, and the current release is downloaded from the GitHub releases page. If a deposit does not appear, updating the wallet and re-checking the account is the first step, followed by the zero-available case in [Why the wallet shows zero available XRP](https://github.com/osmwallet/troubleshooting-hub/blob/HEAD/why-osmwallet-shows-zero-available-xrp.md).

## The mistakes worth naming

Sending on the wrong network is the most expensive one, because a payment on another chain cannot be recovered by the exchange or by the wallet. Sending without a required tag is the most common, and it is recoverable only through the exchange's support with the transaction ID. Sending to a screenshot of an address, rather than the address itself, is the most avoidable.

The habit that prevents all three: copy from the source screen, verify both ends, and test with an amount you would not miss. For a balance leaving an exchange and heading to a device rather than an app, the same steps apply with an extra verification on the device - see *How to move XRP into cold storage, step by step*. For what self-custody changes about the funds once they arrive, *What is a cold wallet for XRP?* and *Should you move your XRP to cold storage?* cover the decision.

### FAQ

### Do I need a destination tag when withdrawing to my own wallet?

No. A tag tells a service which customer a deposit belongs to, and your wallet is identified by its address. Only add a tag if the destination interface shows one.

### Why is my withdrawal smaller than the amount I requested?

The exchange's withdrawal fee is deducted, and on a first deposit part of the balance becomes the account's base reserve. Neither is a wallet charge; both are visible on the ledger once the payment arrives.

### Can an exchange withdrawal be reversed?

No, once it validates. An exchange can reverse a withdrawal it has not yet broadcast, which is one reason to withdraw a test amount first. After the payment is on the ledger, only the receiving account can send it back.

### How long does a withdrawal take?

The ledger settles in seconds; the exchange's processing is the variable. Batching, manual review and first-withdrawal checks can add hours, which is why the test payment is the slowest transaction you will send and the least expensive mistake you can make.
