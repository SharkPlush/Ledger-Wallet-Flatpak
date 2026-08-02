# Ledger-Wallet-Flatpak

Not affilated with the Ledger company in anyway.

Publishing to Flathub won't happen because they want to a compiled from source build which I refuse to do. If Ledger Wallet appears on Flathub one day this will not longer be maintained.

Updates will happen once a month unless someone helps me maintain. (If you open an issue or a PR they'll happen faster.)

For your Linux device to see your Ledger via USB check here under "Linux installation": https://support.ledger.com/article/4404389606417-zd

Or just run.
```
wget -q -O - https://raw.githubusercontent.com/LedgerHQ/udev-rules/master/add_udev_rules.sh | sudo bash
```
Whatever you're comfortable with.

To build run:
```
flatpak run org.flatpak.Builder --force-clean --repo=ledger-wallet-community-flatpak build-dir com.ledger.wallet.yml
```

TODO:

1. Stop relying on device=all and find a more secure way to allow the physcial Ledger wallet to communicate over USB.
