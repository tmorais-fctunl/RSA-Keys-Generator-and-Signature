This README was last updated on October 2nd 2024.
This project was developed as part of a research dissertation at NOVA SST/FCT.

# RSA-Keys-Generator-and-Signature
This notebook allows the generation of N RSA keys and the signing of any message using SHA256 and PKCS1v15.
You can change the endianess of the signature but be cautious of this option if using the signatures in another system.

We plan in the future to permit different hashing and signing algorithms.

# Requirements
- Python >3.8
- Pycryptodome library

# How to use

- RSA_Generate allows you to generate several RSA keys which can then be writen in a file;
- RSA_PKCS1_v1_5_Sign allows you to sign some input with an RSA key. A json file is writen with the public key, hash and signature, as big integers.
- Circom Input Builder will write a JSON file that serves as input to the Efficient and Strong group signature circuits used [here](https://github.com/tmorais-fctunl/Circom-group-rsa-verify)
