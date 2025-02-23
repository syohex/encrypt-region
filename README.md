# encrypt-region

<p>
    <a href="https://melpa.org/#/encrypt-region"><img alt="MELPA" src="https://melpa.org/packages/encrypt-region-badge.svg"/></a>
</p>

An Emacs package for encrypting and decrypting arbitrary regions.

## Getting started

* Get encrypt-region.
* Add the following to your .emacs config:

```elisp
(require 'encrypt-region)
```

* Set your 32-hexchar secret key:

```elisp
(setq encrypt-region-key "<your key here>")

;; Example: (setq encrypt-region-key "616461746120646e6d20726f20656164") 
```

* Encrypt a region using ```M-x encrypt-region-encrypt```
* Decrypt an encrypted region using ```M-x encrypt-region-decrypt```

## Notes

Authenticated encryption is used by default using ChaCha20-Poly1305 from GnuTLS.
