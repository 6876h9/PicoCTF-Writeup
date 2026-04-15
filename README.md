# PicoCTF-Writeup

# 13 — ROT13

**Category:** Cryptography  
**Author:** Alex Fulton / Daniel Tunitis  
**Platform:** picoCTF  

---

## Challenge

```
cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}
```

Decode the ciphertext using ROT13.

---

## Solution

ROT13 shifts each alphabetical character by 13 positions. Since the alphabet has 26 letters, applying it twice returns the original — it is its own inverse.

Decode via terminal:

```bash
echo "cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```

---

## Flag

The flag is stored in [`flag.txt`](./flag.txt).
