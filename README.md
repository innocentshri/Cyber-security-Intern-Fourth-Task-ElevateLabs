# Task 4 - Password Security & Authentication Analysis

## Objective 
The goal of this task is to understand how passwords are stored, how weak passwords can be attacked, and how strong authentication mechanism protect systems from unauthorized access.

--- 

## Tools used
- Hash concepts - MD5, SHA, bcrypt
- Online hash identifiers
- Study reference of tool like Hashcat and John the Ripper

---

## What is Hashing? 
Hashing is a one-way process that converts a password into a fixed-length stirng called a hash.

Example
password → 5f4dcc3b5aa765d61d8327deb882cf99

---

## Difference Between Hashing and Encryption

| Hashing | Encryption |
|------|-----------|
| One-way process | Two-way process |
| Cannot be reversed | Can be decrypted |
| Used to store passwords | Used to protect data |
| More secure for authentication | Used for data confidentiality |

---

## Hash Types Studied
- **MD5** → Fast but insecure
- **SHA-1** → Better than MD5 but still weak
- **bcrypt** → Secure, slow, recommended

---

## Sample Weak Password Hashes

| Password | Hash (MD5) |
|--------|-----------|
| password | 5f4dcc3b5aa765d61d8327deb882cf99 |
| 123456 | e10adc3949ba59abbe56e057f20f883e |

These passwords are weak because:
- They are common
- They exist in wordlists
- They can be cracked quickly

---

## Brute Force vs Dictionary Attack

| Brute Force Attack | Dictionary Attack |
|------------------|------------------|
| Tries all combinations | Uses known password lists |
| Very slow | Very fast |
| Guaranteed success | Efficient for weak passwords |

---

## Why Weak Passwords Fail
- Short length
- Predictable patterns
- Common words or numbers
- Used on multiple sites

---

## What is MFA?
MFA adds extra security layers:
1. Something you know → Password
2. Something you have → OTP, mobile
3. Something you are → Fingerprint, face

Even if a password is stolen, MFA blocks access.

---

## What Makes a Strong Password?
- At least 12 characters
- Random combination
- Mix of:
  - Uppercase
  - Lowercase
  - Numbers
  - Symbols

Example:
X7@Lq#9M!Z2a

---

## Security Recommendations
- Never store passwords in plain text
- Use bcrypt or Argon2
- Enforce strong password policies
- Enable MFA
- Limit login attempts
- Use password managers

---

## Final Outcome
This task helped me understand:
- How passwords are attacked
- Why weak passwords fail
- How strong authentication protects systems
---

## Awareness of Password Cracking Tools

Although real password cracking should only be done in controlled lab environments, tools like the following are commonly used in cybersecurity:

- **Hashcat**
  - GPU-based password cracking tool
  - Supports dictionary and brute force attacks
  - Used for security testing

- **John the Ripper**
  - CPU-based password cracking tool
  - Simple and widely used
  - Good for learning password security

These tools are used only for:
- Testing password strength
- Auditing systems
- Educational purposes

