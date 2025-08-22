# E2E-Encryption-Demo
This interactive demo simplifies end-to-end encryption for educational purposes, showing how two people can secretly agree on a shared key. For simplicity, random integers between 1 and 10 are used for these keys. This key is then used to scramble (encrypt) and unscramble (decrypt) private messages, ensuring only the intended recipient can read them.
[Demo Link](https://ronen-sigan.github.io/E2E-Encryption-Demo/)

## How the Encryption Works
This demo uses two simple cryptographic concepts:

### Diffie-Hellman Key Exchange (simplified): 
This process allows two people, like Joe and Jane, to agree on a shared secret key over an insecure channel. Even if a third person sees the exchanged public values, they can't calculate the final shared secret because they don't have the private keys. Our demo uses a simple mod 11 calculation to show how both sides can arrive at the same result independently.
### Vigenère-like Cipher:
This is a more complex substitution cipher that uses the shared secret key to determine a series of shifting values. Instead of a single shift, each letter of the message is shifted by a different amount that repeats in a cycle determined by the key. For real-world encryption, a much more complex and secure algorithm like the Advanced Encryption Standard (AES) is used.
### How to use this demo:
1. Click "Generate Keys" for both Joe and Jane.
2. Click "Calculate Secret" for both. You'll see they have the same secret!
3. Type a message in Joe's text box and click "Encrypt."
4. Click "Send to Jane."
5. On Jane's side, click "Decrypt" to see the original message.

### Acknowledgments
This project was developed with the assistance of an AI coding assistant.
This approach helped in streamlining the development process and generating boilerplate code.
