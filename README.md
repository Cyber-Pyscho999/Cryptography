# Cryptography
Encryption and Decryption of Data
This lab explores multiple classical cryptography challenges inspired by the Krypton wargame series. Each level demonstrates a different encryption or encoding technique, along with the methodology used to break it
🧩 Levels & Solutions Summary
Level 1 — Base64 Encoding
Password: KRYPTONISGREAT  
Base64 is encoding, not encryption. It uses no keys and is easily reversible using public lookup tables.

Level 2 — ROT13 Substitution Cipher
Password: ROTTEN  
ROT13 is a simple rotation cipher. The challenge hinted at a rotation-based substitution, making ROT13 the correct approach.

Level 3 — Caesar Cipher (Chosen-Plaintext Attack)
Password: CAESARISEASY  
Used a chosen‑plaintext attack with the provided encrypt binary.
Key insights:

Caesar cipher shifts letters by a fixed offset.

Using A (position 0) reveals the shift directly.

The binary had setuid permissions, allowing access to the key file.

Symbolic links and a temporary directory were used to redirect output.

Level 4 — Frequency Analysis
Password: BRUTE  
Used English‑language frequency patterns to identify likely plaintext.
Double letters (e.g., VV) helped narrow down possibilities.

Level 5 — Vigenère Cipher (Known Key Length)
Password: CLEARTEXT  
Key: FREKEY  
With the key length known, periodic analysis was used to break the repeating shifts.

Level 6 — Vigenère Cipher (Unknown Key Length)
Password: RANDOM  
Performed frequency analysis across multiple ciphertext samples.
Column scoring revealed the key length (6), allowing decryption.

Level 7 — LFSR (Linear Feedback Shift Register)
Password: LSFRISNOTRANDOM  
Used a custom plaintext attack.
By comparing known plaintext to ciphertext, the repeating LFSR pattern was extracted.
