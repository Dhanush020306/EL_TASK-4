# EL_TASK-4

# PASSWORD SECURITY AND AUTHENTICATION ANALYSIS
In this task we are going to learn about how passwords are stored, about different hash methods,etc....

# Objectives
- Generate password hash
- Identify hash type
- Crack the Hash

# Tools
- Kali linux
- John the Ripper

# Learnings and Practical
**1. How Passwords are Stored?**
  - **Hashing:** A one-way function used for password storage. It cannot be reversed to reveal the original text.
  - **Encryption:** A two-way process that requires a key to decrypt and reveal the original data.

**2. Different Hash Types**
  - **MD5:** 32-character hex string. Fast but weak and deprecated for security; easily cracked.
  - **SHA-1:** 40-character hex string. Also considered weak and vulnerable to modern attacks.
  - **SHA-256:** 64-character hex string. Strong and widely used for modern data integrity.
  - **bcrypt:** Includes a "salt" and cost factor. Very Strong and specifically designed to resist cracking.

**3. Generate Password Hashes**
  - To create a hash for a word run this command *echo -n "password123" | md5sum | awk '{print $1}' > hash.txt* in kali linux
  - <img width="329" height="180" alt="image" src="https://github.com/user-attachments/assets/c776f7b0-a5c5-4c1c-9f54-620bda7cded4" />
