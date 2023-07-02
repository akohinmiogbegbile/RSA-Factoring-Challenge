# RSA Factoring Challenge

Welcome to the RSA Factoring Challenge! This challenge is designed to test your skills in factoring large numbers, a crucial component of the RSA encryption algorithm. In this README file, you will find all the necessary information to understand and participate in the challenge.

## What is RSA?

RSA is a widely used public-key cryptosystem that relies on the difficulty of factoring large composite numbers. The security of RSA encryption is based on the assumption that it is computationally infeasible to factorize the product of two large prime numbers. The RSA Factoring Challenge aims to test and advance the state of factoring technology.

## Challenge Details

The challenge consists of a series of RSA moduli for participants to factorize. Each modulus is a product of two prime numbers, and the goal is to determine those prime factors. The challenge is divided into multiple key sizes, with increasing levels of difficulty.

## Directory Structure

The challenge directory is organized as follows:

```
rsa-factoring-challenge/
  ├── challenges/
  │   ├── key_size_1024/
  │   │   ├── challenge_1.txt
  │   │   ├── challenge_2.txt
  │   │   ├── ...
  │   │   └── challenge_n.txt
  │   ├── key_size_2048/
  │   │   ├── challenge_1.txt
  │   │   ├── challenge_2.txt
  │   │   ├── ...
  │   │   └── challenge_n.txt
  │   └── key_size_4096/
  │       ├── challenge_1.txt
  │       ├── challenge_2.txt
  │       ├── ...
  │       └── challenge_n.txt
  ├── solutions/
  │   ├── key_size_1024/
  │   │   ├── challenge_1.txt
  │   │   ├── challenge_2.txt
  │   │   ├── ...
  │   │   └── challenge_n.txt
  │   ├── key_size_2048/
  │   │   ├── challenge_1.txt
  │   │   ├── challenge_2.txt
  │   │   ├── ...
  │   │   └── challenge_n.txt
  │   └── key_size_4096/
  │       ├── challenge_1.txt
  │       ├── challenge_2.txt
  │       ├── ...
  │       └── challenge_n.txt
  └── README.md
```

- `challenges/`: This directory contains the RSA moduli for each key size. The moduli are stored in separate text files named `challenge_X.txt`, where `X` represents the challenge number.

- `solutions/`: Participants should place their factorization results in this directory. Each solution should be stored in a separate text file named `challenge_X.txt`, corresponding to the challenge number.

## Getting Started

To participate in the RSA Factoring Challenge, follow these steps:

1. Choose a key size you want to tackle (e.g., 1024, 2048, or 4096 bits).

2. Retrieve the modulus from the appropriate challenge file in the `challenges/` directory.

3. Use your factoring algorithm of choice to determine the prime factors of the modulus.

4. Store your solution, listing the prime factors, in a text file named `challenge_X.txt` in the `solutions/` directory.

5. Submit your solution by providing the text file(s) containing the prime factors of the modulus.

## Note

Please note that the RSA Factoring Challenge is designed to be a computationally intensive task, and factoring larger key sizes may require significant computational resources. Feel free to leverage parallel
