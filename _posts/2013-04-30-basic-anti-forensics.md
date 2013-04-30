---
layout: post
title: "Cryptography Basics - How PGP Works"
description: "Basic post outlining the basics of PGP and how it works"
category: "Cryptography" 
tags: ["Cryptography","PGP", "Keys"]
---
{% include JB/setup %}

##PGP - How does it work?
PGP utilizes a comination of some of the best features from conventional and public key cryptography.  It is a *hybrid cryptosystem*.

When a user encrypts data with PGP, it first must compress the plaintext.  Compression saved time and disk space in transmission and more importantly, strengthens it's security.  Most techniques of cryptanalysis involve exploiting patterns found to crack the cipher.  Compressing plain text massively reduces these patterns and is therefore a very effective way of nhancing cryptanalysis resistance.

PGP then makes a session key which expires after it's first (and only) use.  This key is randomly generated from the movements of your moust and the keys that you type.  This ket works with an extremely fast and secure conventional encryptioon algorithm to encrypt the data; the result is ciphertext.  As soon as the data is encrpyted, the session key is encrypted to the recipient's public key and is transmitted along with the ciphertext.

##Decryption
Decryption is the reverse.  The recipient's copy of PGP uses their own pricate key to recover the session key which is then used by PGP to decrypt the ciphertext.