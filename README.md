# Hashing

 ## What is Hashing? 
### Definition (English):
Hashing is the process of converting any input data (text, file, etc.) into a fixed-size string (hash value) using a mathematical function called a hash function.

### Urdu:
Hashing ek technique hai jisme data ko ek fixed-size code mein convert kiya jata hai — isay kehte hain hash. Har input ka unique hash hota hai.

✅ Important: Hashing is one-way – you can’t reverse a hash back to original data.

## Hashing Function
### Definition:
A hash function is a mathematical algorithm that takes input and returns a unique fixed-size output (called hash or digest).

## Properties of Good Hash Functions:
### Property ---------------------------------	Urdu Description

Deterministic ---------------------------------	Har dafa same input ka same hash hota hai

Fast to compute ------------------------------	Quickly result deta hai

Irreversible ----------------------------------	Hash se original data wapas nahi milta

Collision-resistant	-----------------------------Do alag inputs ka same hash na ho

## Common Hashing Algorithms (Hash Functions)

### Algorithm --------------------------------	Output Size -----------------------	Description

MD5 --------------------------------------	128-bit	Fast but not secure, easily broken

(Purana aur weak algorithm hai)

SHA-1 ------------------------	160-bit	Better than MD5, but also broken
(Ab outdated hai)

SHA-256 -------------------------------	256-bit	Part of SHA-2 family, highly secure and widely used

(Aaj kal most secure aur use hone wala algorithm hai)

## Hashing Extension
### Definition:
Hashing extension refers to length extension attacks, where attackers use knowledge of a hash to compute a new hash without knowing the original input.

### Prevention:
Use HMAC (Hash-based Message Authentication Code)
HMAC = Key + Hash function → prevents tampering

### Urdu:
Kuch weak hash functions (jaise MD5, SHA-1) ko attacker manipulate kar ke naya hash bana leta hai — isay kehte hain hash extension attack. Is se bachne ke liye HMAC use kiya jata hai.

## What is a Digital Signature?
### Definition:
A Digital Signature is a cryptographic technique used to verify the authenticity and integrity of a message, file, or document.

### Urdu:
Digital Signature ek special code hota hai jo batata hai ke:

Data original hai (change nahi hua)

Sender verified hai (real identity)

## How It Works:
1️⃣	Sender creates hash of the message
2️⃣	Sender encrypts the hash using private key = digital signature
3️⃣	Receiver decrypts using sender’s public key
4️⃣	Receiver compares decrypted hash with received hash — if same = valid ✅

## Digital Signature Algorithm (DSA) 

### Definition:
DSA is a mathematical algorithm used to create and verify digital signatures. It uses asymmetric cryptography.

## Important Algorithms for Digital Signatures:

### Algorithm -----------------------------	Description

DSA ----------------------------	U.S. government standard, uses SHA + key pair

RSA ---------------------------	Can be used for both encryption and digital signatures

ECDSA----------------------------	Elliptic Curve version – more secure, shorter keys

**Urdu:**
DSA, RSA, aur ECDSA algorithms se digital signatures bante hain. Inka use data ko sign karne aur uski authenticity check karne ke liye hota hai.

## Summary Table
### Topic ----------------------------------------------------	Description 

Hashing ----------------------------------	One-way data conversion (data ko short, fixed code mein tabdeel karna)

Hash Functions ---------------------------	MD5 (weak), SHA-1 (old), SHA-256 (strong)

Hashing Extension -----------------------------	Attack on weak hash functions; use HMAC to prevent

Digital Signature --------------------------	Verify authenticity and integrity of data

Digital Signature Algorithm ------------------------	DSA, RSA, ECDSA – algorithms for signing and verification
