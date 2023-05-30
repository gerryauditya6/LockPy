# LockPy
LockPy is a Python-based file encryption tool that provides a secure and straightforward way to encrypt your files using strong cryptographic algorithms. This tool allows you to protect your sensitive data by encrypting it with a randomly generated encryption key.

## Features

- Easy-to-use command-line interface
- Strong encryption using the `cryptography` library
- Ability to encrypt files with various extensions
- Securely overwrite the original files with encrypted versions

## Prerequisites

- Python 3.6 or higher
- `cryptography` library

## Installation

1. Clone the LockPy repository to your local machine: 
```
git clone https://github.com/gerryauditya6/LockPy.git
```
2. Navigate to the LockPy directory: 
```
cd LockPy
```
3. Install the required dependencies: 
```
pip install cryptography
```


## Usage

### Encryption

1. Navigate to the LockPy directory.
2. Open the `encryption_script.py` file in a text editor.
3. Locate the following lines:
```python
directory_to_encrypt = 'C:/path/to/your/directory'
target_extensions = ['.txt', '.pdf', '.csv', '.docx', '.mp4']
key_file_path = 'encryption_key.key'
```
4. Change the 'C:/path/to/your/directory' to the full path of the directory you want to encrypt. This directory should contain the files you want to encrypt.
5. Specify the target file extensions to encrypt (e.g., ['.txt', '.docx', '.csv'])
6. Change 'encryption_key.key' to the desired file path where you want to save the encryption key. This is the file that will store the encryption key used to decrypt the files later.

**Note**: Ensure you provide the correct directory path, file extension, and key file path.

7. Save the changes and close the file.
8. Run the encryption script:
```
python encryption_script.py
```
9. The script will encrypt the specified file using a randomly generated encryption key. The original file will be securely overwritten with the encrypted version.

### Decryption

1. Navigate to the LockPy directory.
2. Open the decryption_script.py file in a text editor.
3. Locate the following lines:
```python
directory_to_decrypt = 'C:/path/to/your/directory'
target_extension = ['.txt', '.pdf', '.csv', '.docx', '.mp4']
key_file_path = 'encryption_key.key'
```
4. Change the 'C:/path/to/your/directory' to the full path of the directory you want to decrypt. This directory should contain the files you want to decrypt.
5. Specify the target file extensions to decrypt (e.g., ['.txt', '.docx', '.csv'])
6. Change 'encryption_key.key' to the file path where the encryption key is stored. This should match the key_file_path value used during encryption.

**Note**: Ensure you provide the correct directory path, file extension, and key file path.

7. Save the changes and close the file.
8. Run the decryption script:
```
python decryption_script.py
```
9. The script will decrypt the specified file using the encryption key associated with it. The original encrypted file will be securely overwritten with the decrypted version.

## Specifying Key File Path
By default, the encryption key will be saved to a file named encryption_key.key in the same directory as the script. If you want to specify a different file path for the encryption key, you can modify the key_file_path variable in both the encryption_script.py and decryption_script.py files.

## Security Note
Make sure to securely store and backup the encryption key. Without the key, it will be impossible to decrypt the files.

## Contributing
Contributions are welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.

