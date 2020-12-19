# PotOfCoffee2Go Encrypted Steganography Server

This steganography server not only hides messages in images, it also encrypts the messages embedded in the images. The underlying grunt work are [@mykeels/steganography][1] which is inspired by [rodrigouroz/steganography][2].

Messages can be plain text, Markdown, or an HTML document. The passphrases used to encrypt/decrypt messages are used on-the-fly and **NOT STORED ANYWHERE**, server or client side. (Thus, if you or recipient forget the passphase applied to an image - good luck  on decrypting the message!)

>“Just because you're paranoid doesn't mean they aren't after you.”
>     ― Joseph Heller, Catch-22

The server can be run exposed to the web (public) or as `localhost` (private). The most secure is to run the server private... but requires both the sender and receipiant to install the server on their local computers. Which is a no-brainer...

Must have [git][3] and [nodejs][4] installed.

```
git clone tobedetermined
cd stegano-server && npm install
npm start
```

[1]: https://github.com/mykeels/steganography
[2]: https://github.com/rodrigouroz/steganography
[3]: https://git-scm.com/
[4]: https://nodejs.org/