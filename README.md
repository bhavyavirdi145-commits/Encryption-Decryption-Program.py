# Encryption & Decryption Program (Python)

A simple yet effective Python-based encryption and decryption program using a **substitution cipher algorithm** with a randomly generated key. This project demonstrates fundamental cryptographic concepts and character mapping techniques.

## Features

- Randomized substitution cipher key generation
- Encrypts plaintext into unreadable format
- Decrypts encrypted text back to original
- Supports:
  - Alphabets (A-Z, a-z)
  - Numbers (0-9)
  - Special characters
- Beginner-friendly implementation of cryptography

## Tech Stack

- Python 3
- Built-in libraries:
  - `random`
  - `string`

## Project Structure

Encryption-Decryption-Program/
│
├── Encryption Decryption Program.py
└── README.md

## How It Works

This program uses a **Substitution Cipher**, where:
- A list of characters is created
- A shuffled version of this list acts as a key
- Each character is replaced with its mapped counterpart

## Program Flow

Start
↓
Initialize Cipher Class
↓
Generate Character Set
↓
Shuffle Key
↓
Take User Input (Plaintext)
↓
Encrypt Text
↓
Display Encrypted Output
↓
Take Encrypted Input
↓
Decrypt Text
↓
Display Original Text
↓
End

## Code Architecture

Cipher Class
│
├── init()
│ ├── Defines character set
│ ├── Creates shuffled key
│
├── encrypt(plaintext)
│ ├── Maps each character using key
│ ├── Returns encrypted text
│
├── decrypt(encrypted_text)
│ ├── Reverse mapping using key
│ ├── Returns original text
│
main()
│
├── Takes user input
├── Calls encrypt()
├── Calls decrypt()
└── Displays output

### 1. Cipher Class
Handles encryption and decryption logic.

- `__init__()`:
  - Creates character set
  - Generates shuffled key

- `encrypt(plaintext)`:
  - Maps each character using substitution

- `decrypt(encrypted_text)`:
  - Reverses mapping to original text

### 2. Main Function

- Initializes cipher object
- Takes user input
- Calls encryption & decryption methods
- Displays results

## Pseudocode

### Encryption

START
Create list of characters
Shuffle characters to create key
FOR each character in plaintext:
IF character exists in list:
Replace with corresponding key character
ELSE:
Keep character unchanged
RETURN encrypted text
END

### 🔓 Decryption


START
FOR each character in encrypted text:
IF character exists in key:
Find index in key
Replace with original character from list
ELSE:
Keep character unchanged
RETURN decrypted text
END

## How to Run

1. Clone the repository:

git clone https://github.com/your-username/encryption-decryption-program.git


2. Navigate to the project folder:

cd encryption-decryption-program


3. Run the program:

python "Encryption Decryption Program.py"

## Example


Input: Hello123!
Encrypted: Xy#9@Lm2$
Decrypted: Hello123!

## Limitations

- Encryption key is randomly generated each run
- Cannot decrypt previous outputs without same key
- Not suitable for real-world secure encryption


## Future Improvements

- Save/load encryption key
- GUI interface (Tkinter)
- File encryption support
- Advanced encryption algorithms (AES, RSA)


## Author

- Bhavya Virdi
- 25BOE10010
- VIT Bhopal University
  
## License

This project is open-source and available under the MIT License.

<img width="1029" height="267" alt="Screenshot 2026-03-28 204107" src="https://github.com/user-attachments/assets/3aafcfa6-21de-4451-9247-8def49843dec" />

