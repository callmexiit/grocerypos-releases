# GroceryPOS releases

Update packages for [MANA.DEV GroceryPOS](https://mana.dev). No source here -
only the installers a shop downloads.

Each package is verified before it is installed. The till holds the vendor's
Ed25519 public key, reads a **signed manifest** naming the version, the address
and the SHA-256, checks that signature, then checks the bytes it downloaded
against that hash. The address is plumbing: serving a different file here
cannot make a till install it.

| File | Version |
| --- | --- |
| `GroceryPOS_Update_1.0.1.exe` | 1.0.1 |
