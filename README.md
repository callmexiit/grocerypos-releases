# GroceryPOS releases

Update packages for MANA.DEV GroceryPOS. No source here - only the installers
a shop downloads.

Each package is verified before it is installed. The till holds the vendor's
Ed25519 public key, reads a **signed manifest** naming the version, the address
and the SHA-256, checks that signature, then checks the bytes it downloaded
against that hash.

So the address is only plumbing. Putting a different file here cannot make a
till install it, and uploading a package changes nothing until the matching
manifest is signed and published.

| File | Version |
| --- | --- |
| `GroceryPOS_Update_1.0.2.exe` | 1.0.2 |
| `GroceryPOS_Update_1.0.1.exe` | 1.0.1 |
| `GroceryPOS_Update_1.0.0.exe` | 1.0.0 |
