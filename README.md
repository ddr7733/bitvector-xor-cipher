# bitvector-xor-cipher

Implementation of XOR cipher with Zero Padding using BitVector library.  
Educational project demonstrating symmetric encryption, one-time pad principles, and block alignment techniques.

##  For educational purposes only

## Overview

This project implements a simple XOR-based symmetric cipher. It reads arbitrary input (text or file), applies zero padding to align data to 128-bit blocks, and encrypts it using a cryptographically secure random key generated with Python's `secrets` module.

## How It Works

1. **Input**: Text string or binary file
2. **Padding**: Zero padding applied to reach 128-bit block alignment
3. **Key Generation**: Random key longer than plaintext by 32 bytes (256 bits)
4. **Encryption**: Bitwise XOR operation (`cipher = data ^ key`)
5. **Output**: Key saved as `.bin`, ciphertext saved as `.hex`

## Features

- XOR cipher following one-time pad principles
- Zero padding for block alignment
- Cryptographically secure key generation via `secrets`
- Bit-level operations using `BitVector` library
- Supports both plaintext strings and binary files

## Files

| File | Description |
|------|-------------|
| `xor_encrypt.py` | Encryption script |
| `xor_decrypt.py` | Decryption script |


## Requirements

- Python 3.6+
- BitVector library

## Installation

```bash
pip install BitVector
Disclaimer
This cipher is intended for educational demonstration only. It is not suitable for production use. For real-world applications, use established algorithms such as AES-256-GCM.
