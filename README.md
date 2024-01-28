# Vigenère Cipher Implementation

This Python script provides a simple implementation of the Vigenère cipher, a classical encryption technique. The script includes functions for encryption and decryption using a user-defined key.

## Usage

1. **Setup**
    - Ensure you have Python installed on your system.

2. **Running the Script**
    - Open the `vigenere_cipher.py` file in a Python environment or text editor.

3. **Encrypting a Message**
    - Modify the `text` variable with the message you want to encrypt.
    - Modify the `custom_key` variable with your desired encryption key.
    - Run the script.
    - The encrypted message will be displayed in the console.

4. **Decrypting a Message**
    - Use the same `custom_key` used for encryption.
    - Call the `decrypt` function with the encrypted message and the key as arguments.
    - The decrypted message will be displayed in the console.
  

## How it Works

- **Key**: The Vigenère cipher uses a keyword or phrase as the key for encryption. This key is repeated cyclically to match the length of the plaintext.

- **Encryption**: Each letter in the plaintext is shifted cyclically based on the corresponding letter in the key. This creates a polyalphabetic substitution, making it harder to break the encryption.

- **Decryption**: To decrypt, the receiver uses the same keyword and shifts the ciphertext letters in the reverse direction to reveal the original plaintext.

## Example

- **Plaintext**: "HELLO"
- **Keyword**: "KEY"
- **Encrypted**: "VIQRQ"
- **Decrypted**: "HELLO"

In this example, the plaintext "HELLO" is encrypted using the keyword "KEY" to produce the ciphertext "VIQRQ". Decryption using the same keyword yields the original plaintext "HELLO".


## Note

- This implementation supports only lowercase alphabetic characters. Non-alphabetic characters remain unchanged.
- The Vigenère cipher is susceptible to known-plaintext attacks and chosen-plaintext attacks and is not recommended for secure communication.
