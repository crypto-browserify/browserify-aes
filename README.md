# browserify-aes
[![Build Status](https://travis-ci.org/crypto-browserify/browserify-aes.svg)](https://travis-ci.org/crypto-browserify/browserify-aes)

Node style aes for use in the browser.
Implements:

 - createCipher
 - createCipheriv
 - createDecipher
 - createDecipheriv
 - getCiphers

In node.js, the `crypto` implementation is used, in browsers it falls back to a pure JavaScript implementation.

`EVP_BytesToKey` is a straight up port of the same function from OpenSSL as there is literally no documenation on it beyond it using 'undocumented extensions' for longer keys.

## LICENSES
Much of this library has been taken from the AES implementation in [triplesec](https://github.com/keybase/triplesec) (apparently licensed MIT),  which is a partial derivation of [crypto-js](https://code.google.com/p/crypto-js/), which is licensed BSD-3 clause, the relevant LICENSE text for both MIT and BSD-3 can be found in [LICENSE](LICENSE).

Parts of `ghash.js` are a partial derivation of work by Juho Vähä-Herttua in [SJCL](https://github.com/bitwiseshiftleft/sjcl),  which is LICENSED `BSD-2 || GPL-2`,  with the LICENSE text included inline in `ghash.js`.
