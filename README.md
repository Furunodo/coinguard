# coinguard

vaporware: python script to watch addresses to see if coins move


## Problem

An attacker managed to get hold of your private key and starts moving funds.

You only find out when you check your wallet, whether that's watch only or the real thing.

If you knew much faster there's a way to recover some of your funds. For example, if you have different types of wallets based on one private key, or you are using a BIP39 passphrase.


## Proposed solution

A simple Python script that checks addresses of your wallets that will send out a warning in case funds move.

The script can (should) run on the same machine running your full node to mitigate privacy issues.



