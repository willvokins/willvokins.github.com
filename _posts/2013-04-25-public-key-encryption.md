---
layout: post
title: "Public Key Encryption"
description: ""
category: 
tags: ["Keys","Cryptography","Diffie","Hellman"]
---
{% include JB/setup %}

##Public Keys
The dilemmas people face with key distribution daily are solved by Diffie & Hellman's 1975 *public key cryptography*.  Public Key Cryptography is an asymmetric scheme that uses two keys for an encryption, rather than one.  The keys it uses are as follows:
- **Public Key** - Public keys are used to *encrypt* data.
- **Private Key** - Private keys are used to *decrypt* data.
You are supposed to publish your public key to the world and keep your private key under wraps.  Anybody with a copy of your public key can only encrypt information for you to read.  **Anybody**.

It is literally *impossible* to pull a private key from a public key, making it intensely difficult to decrypt.  The only people that can decrypt the data are those with the private key you have given them.  Bruteforcing is possible, but rarely accurate and takes a **very, very long time**.

![Cryptography Graph](http://i.msdn.microsoft.com/dynimg/IC155063.gif)

**Image Source**: Microsoft