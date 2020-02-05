# coinguard

vaporware: python script to watch addresses to see if coins move


## Problem

An attacker managed to get hold of your private key and starts moving funds.

You only find out when you check your wallet, whether that's watch only or the real thing.

If you knew much faster there's a way to recover some of your funds. For example, if you have different types of wallets based on one private key, or you are using a BIP39 with one or more passphrases.


## Proposed solution

A simple Python script that checks addresses of your wallets that will send out a warning in case funds move.

The script can (should) run on the same machine running your full node to mitigate privacy issues.

### Example scenario

`coinguard` can work well if you use the BIP39 format to store your private key, and then use an additional passphrase
If you leave a small amount in a wallet without a passphrase it's likely that attackers who get access to your
hardware wallet or paper backup (that doesn't hold the passphrase) will move the funds as soon as possible.
Now if you run `coinguard` every 10 minutes you will get a notification within a short time and depending on your
setup you may be able to still move the funds in your passphrase protected wallet.


