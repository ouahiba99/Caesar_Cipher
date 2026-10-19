# 🔐 Caesar Cipher — Python

A lightweight Python command-line tool for encoding and decoding messages using the **Caesar cipher**, a classical substitution cipher that shifts letters by a specified number of positions in the alphabet.

## ✨ Features

- **Encode messages:** Transform plaintext into ciphertext.
- **Decode messages:** Recover the original message using the same shift value.
- **Custom shift:** Choose an offset between 1 and 26.
- **Case preservation:** Maintain uppercase and lowercase letters.
- **Character preservation:** Keep spaces, numbers, punctuation, and special characters unchanged.
- **Simple CLI:** Interact with the program directly through your terminal.

## 🧠 How It Works

The Caesar cipher substitutes each letter with another letter a fixed number of positions away in the alphabet. When the shift reaches the end of the alphabet, it wraps around to the beginning.

For example, with a shift of `3`:

| Plaintext | Ciphertext |
|---|---|
| A | D |
| B | E |
| C | F |
| X | A |
| Y | B |
| Z | C |

The implementation uses Python's built-in `str.maketrans()` and `str.translate()` methods to create and apply character mappings.

- **Encoding:** Shifts letters forward by the selected offset.
- **Decoding:** Reverses the mapping using the same offset.

## 🛠️ Technologies

- Python 3
- Python standard library
- Command-line interface (CLI)

No external dependencies are required.

## 🚀 Getting Started

### Prerequisites

Make sure Python 3 is installed on your system.

Check your version:

```bash
python3 --version
```

### Installation

Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/ouahiba99/Caesar_Cipher.git
cd Caesar_Cipher
```

### Run the Program

Execute the Python script containing the cipher implementation:

```bash
python3 <script_name>.py
```

Replace `<script_name>.py` with the actual name of your Python file.

## 💻 Usage

When the program starts, choose whether to encode or decode a message.

### Example 1: Encoding

```text
Choose [e]ncode or [d]ecode: e
Enter your plaintext message: Hello World
Choose the shift (1-26): 3

Your encoded message: Khoor Zruog
```

### Example 2: Decoding

```text
Choose [e]ncode or [d]ecode: d
Enter your ciphertext message: Khoor Zruog
Choose the shift (1-26): 3

Your decoded message: Hello World
```

### Input Validation

The program accepts shift values from `1` to `26`. Values outside this range raise an exception. The operation must be either `e` (encode) or `d` (decode).

## 🔒 Security Considerations

The Caesar cipher is a historical encryption technique, not a secure modern cryptographic algorithm. Its small key space makes it vulnerable to brute-force attacks and frequency analysis.

This implementation is intended for educational purposes and experimentation with basic cryptographic concepts, not for protecting sensitive information.

## 🎯 Learning Objectives

This project demonstrates:

- Python functions and parameters
- String manipulation and character translation
- User input and conditional statements
- Basic input validation
- Encoding and decoding logic
- Fundamentals of classical substitution ciphers

## 👩‍💻 Author

**Ouahiba Ahmid**

GitHub: [@ouahiba99](https://github.com/ouahiba99)

## 📂 Repository

[Caesar_Cipher — GitHub Repository](https://github.com/ouahiba99/Caesar_Cipher)

