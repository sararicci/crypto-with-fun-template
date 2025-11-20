# 🔐 Group 6 – Symmetric Cryptography: Stream Ciphers and Hash Functions

Welcome to our project!  
This page contains our 2 interactive exercises on **[Symmetric Cryptography: Stream Ciphers and Hash Functions]**. Each exercise is built with a different tool (Kahoot, Miro, Other).

---

## 📘 Topic: Symmetric Cryptography

### 🟢 Exercise 1 – Kahoot Quiz
- **Tool**: Kahoot 
- **Link**: [Play the quiz](https://create.kahoot.it/share/hash-functions/1c633b8a-1f01-4f96-a5f8-4644893b619a)  
- **Description**: A short 5-question interactive quiz testing your knowledge of hash functions in real-world scenarios. Challenge yourself on topics like file integrity verification, password storage, and cryptographic security.
#### **Crypto concept explained**:  

**Hash functions** are one-way mathematical algorithms that transform input data of any size into a fixed-size output (hash/digest). 
They are fundamental to modern cryptography and have three key properties:

1. Deterministic: Same input always produces the same hash
2. One-way: Cannot reverse the hash to get original input
3. Collision-resistant: Nearly impossible to find two different inputs with the same hash

**Real-world applications**:

🔒 File Integrity: Verify downloaded files haven't been tampered with (SHA-256 checksums)
🔑 Password Storage: Store hashed passwords instead of plaintext (bcrypt, Argon2)
⛓️ Blockchain: Link blocks together and ensure immutability (Bitcoin uses SHA-256)
🔧 Version Control: Git uses SHA-1 to identify commits and detect corruption
📜 Digital Signatures: Create message digests for signing documents

Common hash algorithms: MD5 (deprecated), SHA-1 (deprecated), SHA-256 (current standard), SHA-3, bcrypt, Argon2


---

### 🔵 Exercise 2 – Miro Puzzle
- **Tool**: Miro  
- **Link**: [Solve the puzzle](https://miro.com/...)  
- **Description**: Drag-and-drop game where students match numbers to their modular inverses in **ℤ₁₄***.  
- **Crypto concept explained**:  
  The concept of *inverses* is central to modular groups, ensuring decryption can reverse encryption.

---

## 📝 Summary
Through these 3 exercises, we explored:  
- Modular arithmetic basics.  
- Inverses in multiplicative groups.  
- Exponentiation in cryptography.  

---

