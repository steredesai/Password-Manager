# Password Manager 🔐

## Background

Password security is a crucial aspect of cybersecurity, and this project aims to develop a password manager that not only securely stores passwords but also encrypts them with a key to enhance the security of stored credentials. The implementation includes strong encryption mechanisms and a user-friendly command-line interface (CLI) for interaction.

## Objectives

The main objectives of the password manager are:

- Create a secure password manager that saves and encrypts user credentials.
- Utilize strong encryption mechanisms such as SHA-256 hashing and bitwise XOR encryption.
- Provide features for adding, retrieving, and modifying passwords.
- Implement a secure and user-friendly CLI for user interaction.

## Scope

The project focuses on developing a password manager that securely stores and encrypts passwords provided by the user. It uses a command-line interface (CLI) to handle operations like adding new users, managing passwords, and retrieving or updating stored passwords. Passwords are stored in a text file with encryption applied for added security.

## Implementation

### Encryption Functions

The encryption functions handle encryption and decryption techniques using cryptographic methods. SHA-256 hashing and bitwise XOR encryption are employed for secure password encryption.

### Password Management Functions

These functions allow users to create, retrieve, and update passwords. They include:

- **Add Function:** Encrypts the password and saves it in the file in binary append mode.
- **Retrieve Function:** Given a username and an encryption key, retrieves and decrypts the user's password from the file.
- **Update Function:** Checks if the username exists in the file, encodes the new password, and replaces the old password.

### Main Application Logic

The main application logic provides a command-line interface (CLI) for user interaction. Users can select options to add, retrieve, or update passwords.

### Libraries Used

- **os library:** Used for file handling functions and directory operations.
- **hashlib library:** Provides a secure way to generate hash values for data like strings, files, or binary data.

## How to Use

1. Clone the repository to your local machine.
2. Open a terminal and navigate to the project directory.
3. Run the password manager using the command-line interface.

```bash
python password_manager.py
```

Follow the on-screen instructions to perform password management operations.
