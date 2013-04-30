---
layout: post
title: "Cryptography - Keys"
description: ""
category: 
tags: []
---
{% include JB/setup %}

##What are Keys?
Keys are values that work with a cryptographic algorithm to generate and produce a specific ciphertext.  They are essentially just huge numbers.  Key size is measured in bits - the number representing a 1024-bit key for example is pretty huge.  In public key cryptography, the bigger the key, the more secure the ciphertext.

However, key size with public keys are completely unrelated to conventional encryption's secret key. A conventional 80-bit key has the strength of a 1024-bit public key.  Once more, the bigger the key, the more secure.  The algorithms on the other hand are very different.

While public keys and private keys are mathematically related, it is very difficult to unmask the private key when you only have the public key.  However this does not mean it's *impossible*.  Infact it's highly possible, given that you have enough of two things:

- Time
- Computing Power

This makes it essential for you to pick keys of the right size - large enough to be secure but small enough to be applied quickly and efficiently.  You may also need to consider who might be trying to read your files - How determined are they?  Do they have the necessary power?  What are their ambitions and to what extent will they go?

Larger keys will be secure for a much longer time, If what you want to encrypt must be hidden for many years - you would definitely need to use a very large key.  Saying that, we are completely unaware of how the future's technology will be able to determine keys.  Will we even be using the same methods in the years to come?

