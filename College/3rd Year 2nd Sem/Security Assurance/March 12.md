# Cryptography
## 2 Components
1. Encryption
	- Practicing of hiding message
2. Authenticity & Integrity
	- Ensuring thay data has not been altered

## Encryption Algorithms are standardized and published
### Caesar Cipher
- Named after Julius Caesar, who used it with a shift of three to protect messages of military significance
- Pros
	1. Simple
	2. Easy to implement
- Cons
	1. The encryption and decryption algorithms are known
	2. There are only 25 keys to try (vulnerable to brute-force attack)
	3. The language of plaintext is known and easily recognized

### Playfair Cipher
- playfair square or Wheatstone-Playfair cipher
- manual symmetric encryption technique
- first literal diagram substitution cipher
- invented in 1854 by Charles Wheatstone
- Multiple letter encryption cipher
- Diagrams
- 5x5 constructed using a keyword. (Ex. CIPHER)

#### Rules for Encryption
1. Diagram (5x5)
2. I & J are combined
3. Repeating letters - Filler letter (X)
4. Same column downwards: wrap around 
5. Same row to the right: wrap around
6. Rectangle / square: swap

#### Rules for Decryption
1. Diagrams (5x5)
2. I & J is combined
3. Same column upward: wrap around
4. Same row to the left: wrap around
5. Rectangle / square: swap