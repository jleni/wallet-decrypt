# Bitcoin Wallet Decrypt (BackupFile -> Mnemonic)

If you have been using the Bitcoin Wallet from *Bitcoin Wallet developers*, it is likely you want to get your Bitcoin Cash or take control of your private keys.

I wrote this script to simplify this process for myself. This script will obtain a BIP-39 mnemonic that can later be used to transfer Bitcoin or Bitcoin Cash to other wallets.

**WARNING: You will be decrypting your wallet so the private key (mnemonic) might be compromised.**

## Instructions

- Go to `Safety` and remove the spending PIN.
- Backup your wallet. Remember the password you use.
- Connect your phone with a usb cable and copy the backup file.

Dependencies
```
pip install pycrypto
```

Run the script (replace with the appropriate filename and password)
```
wallet-decrypt.py FILENAME PASSWORD
```

You will get a mnemonic and derivation path that can be used in Electrum / Electrum Cash.

**This software is provided under the Apache License Version 2.0 - Use at your own risk**
