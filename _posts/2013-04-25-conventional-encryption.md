---
layout: post
title: "Conventional Encryption"
description: "Brief tutorial outlining the basics of Conventional Encryption"
category: "Cryptography"
tags: ["Cryptography","Keys"]
---
{% include JB/setup %}

##Conventional Encryption
There are benefits that come with conventional encryption.  It is quick and is especially useful for static data.  However, conventional encryption alone can be very difficult and rather inconvenient, simply because it is a pain to securely distribute the decryption key.

For two people to communicate securely using conventional encryption, they must both agree upon a secure key and keep it between themselves.  If they are (physically) very far away from each other, they will need a courier; a mobile phone or secure email to prevent the disclosure of the key during transmission.  Anybody who gains access to the key, gains access to *your data*.  The main and persistent problem with conventional encryption is key distribution:  How do you send the key to the other end whilst preventing interception? **Public Key Cryptography**.