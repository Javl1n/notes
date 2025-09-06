# Cryptography
- Art or science of encompassing the principles and methods of transforming an intelligible message unto one that is unintelligible, and re-transform back to original form
- greek word "Krypto's" meaning "Hidden message"
- Study of Hidden/hiding information
- provides Confidentiality, Integrity, and Accuracy.
## Terminologies
- Plaintext
	- message
	- sometimes called cleartext
- Encryption
	- process of disguising a message in such a way as to hide its substance.
- Cipher text
	- encrypted text
- Decryption
	- turning cipher text back into plaintext
- Cipher
	- an algorithm for performing encryption and decryption

Plaintext -> Encryption -> Coded Hex Text -> Decryption -> Plaintext

## Cryptosystem
- an implementation of cryptographic techniques and their accompanying infrastructure to provide information security service.
- also referred as cipher system
### Components of basic cryptosystem
1. Plaintext
2. Encryption Algorithm
3. Cipher Text
4. Decryption Algorithm
5. Encryption Key
6. Decryption Key

- Cryptography
	- science of securing data
- Cryptanalysis
	- science of analyzing and breaking secure communication
	- Classical cryptanalysis:
		- Analytical reasoning
		- application of mathematical tools
		- pattern finding
		- patience
		- Determination
		- luck
- Cryptanalyst 
	- also called attackers
- Cryptology 
	- embraces both cryptography and cryptanalysis 

## Purpose of Cryptography
1. Authentication
	- process if providing one's identity.
2. Privacy / Confidentiality
	- ensuring that no one can read the message except the intended receiver.
3. Integrity
	- assuring the receiver that message has not been altered
4. Non-Repudiation
	- a mechanism to prove that the sender really sent the message

## Types of Cryptography
1. Symmetric cryptography
	- Private Key Cryptography
	- same key used to encrypt and decrypt
2. Asymmetric Cryptograpgy
	- Public Key Cryptography
	- use different keys for encryption and decryption

### Using Keys
#### Private Keys
- used for decrypting

Plaintext - encryption / public key - cipher text

cipher text - decryption / private key - cipher text

- public keys are used for encrypting

## Application of Cryptography
1. Secure Online Transaction
2. Digital Signatures
3. Password Protection

## Encryption Schemes
- Unconditionally Secure
	- if the cipher text does not contain enough information to determine uniquely the corresponding plaintext
- Computationally secure
	- the attacker is investing a lot of time in breaking the cipher text but still can't decrypt the ciphertext.