AES Pocket Calculator
=====================

What would a pocket calculator for doing AES look like?

This is a work-in-progress.

Goals:
An operator should be able to type in a key and encrypt or decrypt payloads.  Mode of operation is up to the operator, 
however it should be doable easily enough.
HMAC is supported too.

The current design facilitates CBC and CTR, and probably more modes.  Documentation on how to use the calculator to do
that is forthcoming.  GMAC might be a nice future feature so that AES-GCM can be used too.

The core computation will be in Rust, so it can run on a microcontroller for an inevitable physical build.
The prototype UI is a webpage, in this repository and you can try it at
https://mcpherrinm.github.io/aescalculator/calculator.html