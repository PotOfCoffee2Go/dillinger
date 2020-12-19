# PotOfCoffee2Go Encrypted Steganography Server

This steganography server not only hides messages in images, it also encrypts the messages embedded in the images.

Messages can be plain text, Markdown, or an HTML document. The passphrases used to encrypt/decrypt messages are used on-the-fly and **NOT STORED ANYWHERE**, server or client side. (Thus, if you or recipient forget the passphase applied to an image - good luck  on decrypting the message!)

The underlying modules that do the grunt work are [@mykeels/steganography][1] which is inspired by [rodrigouroz/steganography][2]

For those that want
[1]: https://github.com/mykeels/steganography
[2]: https://github.com/rodrigouroz/steganography