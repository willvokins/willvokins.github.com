---
layout: post
title: "Cryptography Basics 1"
description: "A breif tutorial outlining the basics of crpyotgraphy."
category: "Cryptography"
tags: ["Cryptography", "Keys", "Caesar"]
---
{% include JB/setup %}

##Encryption and Decryption
Data that can be read and interpreted without any special parameters is known has *plaintext*.  The method of hiding plaintext in such a way as to hide it's value is called *encryption*.  Encrypting plaintext generates unreadable strings known as *ciphertext*.  The main use for encryption is to ensure that information is hidden from anyone who should not be seeing it,  Even if one were to gain access to the information, they would still be at a loss as the data is completely unreadable.

##What is cryptography?
Cryptography is a way of using maths to securely encrypt and decrypt data.  Cryptography enables the user to store sensitive information and transmit it across insecure networks without exposing anything.  Encrypted data is **completely** useless to anyone who does not know how to decrypt it.

*Cryptanalysis* however, is the science behind analyzing and breaking down secure communication.  Typical cryptanalysis involves an interesting combination of analytical reasoning, pattern finding, mathematical tools and determination.

*Cryptology* embraces both Cryptogtaphy and Cryptanalysis.
Conventional 

##Caesar's Cipher
The most popular example of cryptography in history is **Caesar's Cipher**; an encryption method wherein letters were moved around in the alphabet, usually shifted up or down using a *key*.  Say the key is **3**.  The person reading the message would decrypt it by "*shifting*" the alphabet up by three places.  Explanation and example:

####Plaintext
    ABCDEFGHIJKLMNOPQRSTUVWXYZ

####Ciphertext
    DEFGHIJKLMNOPQRSTUVWXYZABC

So... using this key, the ciphertext for the word *VOKINS* would be *YRNLQV*

####Explanation
    0>   V O K I N S
    1>   W P L J O T
    2>   X Q M K P U
    3>   Y R N L Q V

To move from step to step, we change each letter in the word to be one further along.  As the *key* is **3**, we do this **3** times.

*Part two coming soon...*
