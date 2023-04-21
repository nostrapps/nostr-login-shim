

<div align="center">  
  <h1>nostr-login-shim</h1>
</div>

<div align="center">  
<i>nostr-login-shim</i>
</div>

---

<div align="center">
<h4>Documentation</h4>
</div>

---

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/nostrapps/nostr-login-shim/blob/gh-pages/LICENSE)
[![npm](https://img.shields.io/npm/v/nostr-login-shim)](https://npmjs.com/package/nostr-login-shim)
[![npm](https://img.shields.io/npm/dw/nostr-login-shim.svg)](https://npmjs.com/package/nostr-login-shim)
[![Github Stars](https://img.shields.io/github/stars/nostrapps/nostr-login-shim.svg)](https://github.com/nostrapps/nostr-login-shim/)

## Introduction


# Login Shim

A beautiful, client-side login shim that sits on top of a website, requiring users to log in via an extension before viewing the website content. The shim checks for the presence of `window.nostr` and calls `await window.nostr.getPublicKey()` for the login process.

## Installation

To use the login shim in your project, first, download the `index.js` file from this repository and include it in your project folder.

Then, add the following script tag to your HTML file:

```html
<script src="path/to/index.js"></script>
```

Replace path/to with the actual path to the index.js file in your project folder.

## Import from CDN

To import the `awaitnostr` module from a CDN, add the following line to your HTML file:

```JavaScript
import awaitNostr from 'https://cdn.skypack.dev/nostr-login-shim'
```


## Usage

Once you've included the login shim library in your HTML file, it will automatically display the login shim on top of your website content. The shim will remain visible until the user clicks the "Login" button, at which point the library will check for the presence of window.nostr and call await window.nostr.getPublicKey(). If the check is successful, the shim will be hidden, and the user will be able to view the website content.

## Customization

If you need to modify the login process or the appearance of the shim, you can edit the index.js file directly.

For the login process, modify the checkForExtension function as needed. For the appearance, update the shimStyles constant with your desired styles.

## Demo

You can view the demo by clicking [here](https://nostrapps.github.io/nostr-login-shim/test.html).


## License

- MIT
