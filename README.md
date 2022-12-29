# PotOfCoffee2Go Encrypted Steganography Server

This steganography server not only hides messages in images, it also encrypts the messages embedded in the images. The underlying grunt work is done by [@mykeels/steganography][1] which is inspired by [rodrigouroz/steganography][2].

Dependancies are oldies but goldies; [Express][], [Mustache][], [highlightjs][], and [markdown-it][]. They are used to run the site and render the text embedded in images.

Messages can be plain text, Markdown, or an HTML document. The passphrases used to encrypt/decrypt messages are used on-the-fly and **NOT STORED ANYWHERE** - server or client side. (If you forget the passphase applied to an image - your pretty much out of luck  on decrypting the message!)

Images are stored by the server to present a directory list of recently created and viewed images.

Although the server can be run exposed to the web (public), it is ultimately more secure to run as `localhost` (private). The advantage to a public server is the images with encrypted text are available online and users do not need to install the server to create and view messages.

The most secure way to run the server is private and choose a local image to encrypt - then post or email to receipiants. However, that requires that both the sender and receipiant(s) install the server on their local computer.

[git][3] and [nodejs][4] are required to install and run the server.

To install the server ...

```
git clone https://github.../TBD
cd TBD && npm install
npm start
```
If all goes well, in your browser go to `http://localhost:8000` and you are ready to encrypt your first message into an image. (if not goes well... grrr... submit an issue on [github][5]. Your feedback is appreciated.) The port can be changed in the project directory `config.js` - bu more on that later...

> True terror is to wake up one morning and discover that your high school class is running the country.
<br> -- Kurt Vonnegut

You can choose an image from you computer, let's say a pic of what you had for lunch (a Facebook standard) and encrypt a message into it. The image with the text encrypted is displayed and you can right-click 'Save as...' - now post the image your FB wall.

Unbeknownst to most your Facebook 'friends' - the in-plain-site,  totally ignored 'pic of what I had for lunch' contains a sercret message. Might be for your mistress, boy toy, or secret instructions to your lawyer. Pre-arranged they know that any time you post a lunch pic - they Right-click -> 'Save as...' and then decrypt by providing the passphrase and image to 'http://localhost:8000` they installed on their machine,

> Warning: Might not want to use a pic with a kitten in it - will probably go viral! - but still, your message is totally hidden!

[1]: https://github.com/mykeels/steganography
[2]: https://github.com/rodrigouroz/steganography
[3]: https://git-scm.com/
[4]: https://nodejs.org/
[5]: https:/github.com/repo/issues
[6]: https://ngrok.com/
