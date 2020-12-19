# PotOfCoffee2Go Encrypted Steganography Server

This steganography server not only hides messages in images, it also encrypts the messages embedded in the images. The underlying grunt work is done by [@mykeels/steganography][1] which is inspired by [rodrigouroz/steganography][2]. [Mastache][], [highlightjs][], and [markdown-it] are used to render the text embedded in images.

Messages can be plain text, Markdown, or an HTML document. The passphrases used to encrypt/decrypt messages are used on-the-fly and **NOT STORED ANYWHERE**, server or client side. (Thus, if you or recipient forget the passphase applied to an image - good luck  on decrypting the message!)

>“Just because you're paranoid doesn't mean they aren't after you.”
>     ― Joseph Heller, Catch-22

The server can be run exposed to the web (public) or as `localhost` (private). The advantage to a public server is the images with encrypted text are available online. The most secure way to run the server is private and sneaker-net or email encrypted images to receipiants. A private sever requires both the sender and receipiant to install the server on their local computers. Regardless, the system installing the server must have [git][3] and [nodejs][4] installed.

The install for a public server depends on the host provider, do they the support nodejs apps? Well beyond the scope of this README...  Given that, you could look into [ngrok][6] which can expose a private server on your machine to the web. The install for a public server is the same as for a private server - just has an added layer of complexity depending on your host provider.
 
 WTF? - just want to install as a private server and see it work! - so here it is...
 
Installing a private server is a no-brainer...

```
git clone https://github.../TBD
cd TBD && npm install
npm start
```
If all goes well, in your browser go to `http://localhost:8000` and you are ready to encrypt your first message into an image. (if not goes well... grrr... submit an issue on [github][5]. Your feedback is appreciated.)

[1]: https://github.com/mykeels/steganography
[2]: https://github.com/rodrigouroz/steganography
[3]: https://git-scm.com/
[4]: https://nodejs.org/
[5]: https:/github.com/repo/issues
[6]: https://ngrok.com/