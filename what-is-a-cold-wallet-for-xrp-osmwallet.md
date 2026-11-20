<p align="center">
  <img src="assets/banner-article.png" alt="OSM Wallet guide" width="100%">
</p>

# What is a cold wallet for XRP?

A cold wallet keeps the key to your XRP on a device that never connects to the internet, and signs a transaction only when you deliberately connect it. XRP does not require one: a non-custodial software wallet holds the same kind of key. What a cold wallet removes is the exposure that comes with a key stored on a machine you use for everything else.

## What "cold" describes

Cold is a property of where the key lives, not a brand or a product category. If the key is on a device that has no network connection and only signs when asked, that is cold storage. If the key is on a computer, phone or browser that reaches the internet, that is a software wallet - sometimes called a hot wallet - regardless of how carefully it is used.

The distinction is about exposure, so it is worth being precise about what the exposure is. Malware that can read a file on your computer can reach a key stored in an app. Malware cannot reach a key that never leaves a device with no network connection, which is the entire argument for cold storage.

## What a cold wallet removes, and what it does not

A cold wallet removes the possibility that a compromised computer, browser extension or clipboard steals the key. It does not remove the possibility that you lose the device, mistype a destination, approve a payment to a scam address, or store the recovery phrase somewhere exposed. Most reported losses involve the last three rather than a stolen key.

| Risk | Cold wallet | Software wallet |
|---|---|---|
| Key read by malware on your computer | Removed by separation | Possible, reduced by hygiene |
| Device lost or destroyed | Recovery phrase restores access | Recovery phrase restores access |
| Payment sent to a wrong address | Not prevented | Not prevented |
| Recovery phrase photographed or stored online | Not prevented | Not prevented |
| Device screen shows a false address | Prevented when you verify on the device | Not applicable |

The last row is the quiet benefit. A device with its own screen shows the destination where malware on the computer cannot rewrite it, which is why verifying the address on the device is the step that matters most when you use one.

## Does XRP need a cold wallet?

No, and the ledger does not distinguish. Every XRP Ledger account needs a base reserve of 1 XRP to exist, and that applies whether the key is on a device in a drawer or in an app on your desktop. The ledger records the account and its balance; it has no idea how the key is stored, and it offers no extra protection for a cold one.

What differs is your exposure while the key is reachable. If your XRP sits in a wallet you open every day, the key is in the same environment as your email and your downloads. If that environment is ever compromised, the key is a file away from being copied.

## How to tell whether your setup is cold

Three questions settle it, and a single "no" is enough to make the answer software custody.

1. Does the device ever connect to a network? If yes, it is not cold.
2. Does the key exist anywhere other than that device and your written backup? If yes, it is not cold.
3. Does the device show the destination address on its own screen before signing? If not, you cannot verify what you are approving.

A wallet on an old laptop kept offline technically satisfies the first two, and people do run this setup. It is cold in the sense that matters, with the caveat that an offline machine is harder to keep updated and easier to lose track of than a purpose-built device.

If the answer came back no and you want it to be yes, [How to move XRP into cold storage, step by step](https://github.com/osmwallet/beginner-explainers/blob/HEAD/transferring-xrp-into-cold-storage-osmwallet.md) covers moving a balance onto a device.

## Where OSM Wallet fits

OSM Wallet is a non-custodial software wallet for the XRP Ledger, available as a desktop app for Windows, macOS and Linux and as a browser extension. It is not a cold wallet: the key lives on the machine where you installed it. What it offers instead is a desktop surface where ledger work happens - trustlines, issued tokens, swaps, merchant payments - with the key on one machine rather than in a browser profile shared with everything else.

It also pairs with a hardware device, which is how cold storage and daily use combine: the device holds the key and approves each transaction, and the wallet provides the interface and the XRP Ledger features. If your question is whether a software wallet is enough, that pairing is the answer most holders arrive at.

The wallet is actively maintained, and the current release is downloaded from the GitHub releases page. Updating to it is the first step when anything behaves differently from this description.

## Choosing between the two

If you hold a balance you rarely move, cold storage is the honest recommendation - including from a software wallet's own documentation. If you use the XRP Ledger regularly, a software wallet is the one that can do the work. Plenty of holders keep both: a device for the long-term balance, a software wallet for what they actually spend and trade.

For the decision in more detail, see [Cold storage vs software custody: which one you need](https://github.com/osmwallet/beginner-explainers/blob/HEAD/cold-storage-vs-software-custody-osmwallet.md) and [Should you move your XRP to cold storage?](https://github.com/osmwallet/beginner-explainers/blob/HEAD/should-i-move-xrp-to-cold-storage-osmwallet.md). For how theft actually happens, *How XRP gets stolen, and what stops it* is the realistic version, and *What a non-custodial wallet actually means* covers who can move funds in each model.

### FAQ

### Is a cold wallet the same as a hardware wallet?

In practice, yes: a hardware wallet is the usual way to keep a key offline. The concept is the separation, so an offline computer holding a key is also cold storage, just a less practical version of it.

### Can XRP be stored in a cold wallet?

Any XRP Ledger account can be controlled by a key held offline, because the ledger does not care where the key is. The account and its 1 XRP base reserve work identically; only your exposure changes.

### Do I lose my XRP if the cold wallet breaks?

No. The XRP is on the ledger and the account is unchanged. A replacement device plus your recovery phrase restores access, which is why the phrase matters more than the device.

### Should I move all my XRP to cold storage?

Only the part you do not need to use. An account you transact from needs a key that is available, and moving the entire balance offline means reconnecting the device for every payment, trustline or swap.
