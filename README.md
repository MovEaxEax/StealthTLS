# Browser Profiles
This repository contains a JSON file with JA3 and HTTP2 signatures of different browsers to spoof TLS connections.
It also includes some C++ code to load the JSON and save the profiles with structs.

The order of the data matters. So, the headers are in the order, as they would occur in a HTTP2 requests, from top to down, first to last. Same for JA3 ciphers and stuff, index 0 is sent first, last element is sent last.

Some of the headers contain values, for example the encoding or the user agent. The other values are empty and/or can be ignored.

All signatures are ripped from automate.browserstack.com browsers, they offer a lot of different combinations from real devices running browsers on differnt OS.

The C++ code requires the nlohman json library to load the data:
https://github.com/nlohmann/json 

Happy spoofing!


-----------------------------------------------

Tip me a crypto coffee if you like what you see:

BTC:

1FoTxYS2RFKT2a2qWf7UPV1LUdiTuSjTur

LTC:

LTc156KNuD4a9MNH4ZSDgjy6P4uKVsqLqg

DOGE:

DDpYs5xHnT63LvQrdewXNUt8K6VAr1iVbj
