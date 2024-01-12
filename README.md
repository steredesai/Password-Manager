Password Manager 🔐
Background
Password security is an essential component of cybersecurity. Safeguarding user passwords is critical in many applications, including personal accounts and enterprise systems, to protect sensitive information. The goal of this project is to develop a password manager that not only securely stores passwords but also encrypts them with a key, thereby increasing the security of saved credentials.

Objectives
The following are the main objectives of the password manager:

Create a password manager that saves and encrypts user credentials securely.
Use strong encryption mechanisms to safeguard passwords.
Include features for adding, retrieving, and modifying passwords.
Implement a secure and user-friendly command-line interface (CLI) for interaction.
Scope
The project is to develop a password manager that securely stores and encrypts the password given by the user. It uses a command line interface (CLI) to take inputs like adding a new user and passwords and retrieve and update passwords. The passwords are stored in a text file with encryption applied for added security.

Implementation
The key features of the password manager include:

SHA-256 hashing and bitwise XOR encryption are used for password encryption.
New usernames can be added and updated.
Retrieval of previously saved passwords for a specified username.
Replacing old passwords with new ones.
Safely save passwords in a text file.
For each session, a random encryption key is generated.
Components
The main components of the application are as follows:

Encryption functions: These functions handle encryption and decryption techniques using cryptographic methods.
Password Management functions: These allow users to create, retrieve, and update passwords.
Main Application Logic: A command line is included so that the user can provide input through it.
Libraries used:
Os library: Used for file handling functions and directory operations.
Hashlib library: Provides a secure way to generate hash values for data like strings, files, or binary data.
Encryption functions
SHA256 (secure hashing algorithm) is a hash function that takes an input and returns a fixed-size string in bytes. The output is 256 bits long or 32 bytes or 64 hexadecimal characters.

In this program, the password is accepted as input, transformed into bytes, hashed using the SHA-256 algorithm, and the hash is output as a hexadecimal string. This method securely stores passwords by transforming them into a fixed-length string of characters that cannot be easily reversed to disclose the original password.

Password Management functions
Add function: Encrypts the password and saves it in the file in binary append mode. Passwords for all users are stored in this file.
Retrieve function: Given a username and an encryption key, retrieves and decrypts the user's password from the file.
Update function: Checks if the username exists in the file, encodes the new password, and replaces the old password.
Main Application Logic
The main application logic provides a command-line interface (CLI) for user interaction. Users can select whether to add, retrieve, or update passwords.
