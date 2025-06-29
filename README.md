# Python Blockchain Demo

A minimal Python blockchain demo that mines and links blocks using SHA-256 and Proof-of-Work.

## Description

This repository contains a simple Python implementation of a blockchain concept focusing on block creation, mining, and linkage using SHA-256.

Each block includes a `previous_hash`, `data`, a `nonce`, and a `hash`. Blocks are mined using a basic Proof-of-Work algorithm that finds a nonce such that the resulting SHA-256 hash starts with a given number of leading zeros (defined by the difficulty level). 

The script demonstrates:
- How blocks are linked via previous hashes
- How mining adjusts the nonce until a valid hash is found
- The immutability of blocks once mined

## How to Run

1. Make sure you have Python 3 installed.
2. Clone this repository or download the `.py` file.
3. Open a terminal and navigate to the project directory.
4. Run the script:
   ```bash
   python block.py


Example Flow
Block t is created using a fixed genesis hash and mined until its hash starts with four zeros.

Block t+1 is then created using the hash of Block t as its previous hash, and also mined.

Both block hashes are printed to show the linkage and proof-of-work in action.
## Sample Output
Block t hash:    0000ac5100c4b3e2d3d895cd7b457ba7f336fa9bdae68b2e9f8bb14673f4e3bb  
Block t+1 hash:  0000f19dd5d0b77a2f7b6caa766bf553404b7eef5913d525bf883e01408377ad
