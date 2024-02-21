# RSA encryption and signature

## Description

This Python script provides functionalities related to RSA-AOEP encryption, including key generation, encryption, decryption, signature, and signature verification.

## Usage

To run the program, you need to have a Python version equal to or greater than 3.8.1. The script can be used with different options, according to the following instructions:

### Available Options

-   **-i**: Specifies the input file.
-   **-o**: Specifies the output file.
-   **-privkey**: Specifies the path to the file containing the private key.
-   **-pubkey**: Specifies the path to the file containing the public key.
-   **-encrypt**: Enables the encryption operation.
-   **-decrypt**: Enables the decryption operation.
-   **-sign**: Enables the signature operation.
-   **-verify**: Enables the signature verification operation.
-   **-genkeys**: Enables the generation of a key pair.
-   **-signature**: Specifies the file containing the signature.

### Usage Examples

1. **Key Generation:**

    ```bash
    python main.py -genkeys
    ```

2. **Encryption:**

    ```bash
    python main.py -encrypt -i input.txt -o output.rsa -privkey private_key.pem
    ```

3. **Decryption:**

    ```bash
    python main.py -decrypt -i output.rsa -o output.txt -pubkey public_key.pem
    ```

4. **Signature:**

    ```bash
    python main.py -sign -i input.txt -o input.sign -privkey private_key.pem
    ```

5. **Signature Verification:**
    ```bash
    python main.py -verify -i input.txt -signature input.sign -pubkey public_key.pem
    ```

## Dependencies

    pip3 install rsa
    pip3 install cryptography
