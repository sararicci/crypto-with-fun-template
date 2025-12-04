# 🔐 Group SKYTALE – Crypto with Fun!

Welcome to our project!  
This page contains our 3 interactive exercises on **[chosen topic: Random Number Generation]**.  
Each exercise is built with a different tool (Wayground Quiz, Miro, Other).

---

## 📘 Topic: Random Number Generation

### 🟢 Exercise 1 – Wayground Quiz (Joshua Nwokoye)
- **Tool**: Wayground
- **Link**: [Play the quiz](https://wayground.com/print/quiz/6919a42202063608ba3be1b1)
- **Description**: A comprehensive 13-question quiz focusing on Cryptographically Secure PRNGs and the Blum Blum Shub algorithm.
- **Crypto concept explained**:
  This exercise details the rigorous standards for a Cryptographically Secure PRNG (CSPRNG), emphasizing the importance of the next-bit test and forward security to prevent state prediction. It specifically examines the Blum Blum Shub algorithm, testing knowledge of its recurrence relation ($x_{n}=x_{n-1}^{2} \mod m$), the method for extracting random bits (using the least significant bit), and the formula for direct computation. Furthermore, it highlights the critical role of using TRNGs for generating unpredictable seeds and the use of statistical methods like the Frequency Test to detect potential weaknesses in the output.

---

### 🔵 Exercise 2 – Miro Puzzle (Lungu Masauso)
- **Tool**: Miro
- **Link**: [Solve the puzzle](https://miro.com/...)
- **Description**: An interactive quiz using sticky notes to test knowledge on PRNG mechanisms and mathematical calculations.
- **Crypto concept explained**:
  This exercise focuses on the internal mechanics of random number generators. It tests understanding of the **Linear Congruential Generator (LCG)** by asking for its recurrence relation and requiring a manual calculation of the next state ($X_1$) given specific parameters ($m, a, c, X_0$). It also explores the **Mersenne Twister**, specifically questioning why it is considered **cryptographically insecure** (due to predictability) and what operations it uses. Furthermore, the puzzle covers the **Blum Blum Shub** recurrence relation and fundamental concepts like the role of a **seed**, the **period** of a generator, and common **statistical tests** for randomness.

---

### 🟣 Exercise 3 – Kahoot (Arun Chittuparambil Polson)
- **Tool**: Kahoot
- **Link**: [Try it here](https://kahoot.com/...)
- **Description**: A multiple-choice quiz covering the classification, properties, and applications of random number generators.
- **Crypto concept explained**:
This exercise assesses the understanding of **Random Number Generator (RNG)** classifications, specifically distinguishing between **True Random Number Generators (TRNG)**, which rely on physical randomness, and **Pseudo-Random Number Generators (PRNG)**, which use deterministic algorithms. It highlights essential properties of a good PRNG, such as **uniformity and independence**, and explores **Shannon's Entropy** as a measure of a sequence's unpredictability. Additionally, the quiz covers practical aspects, including **post-processing techniques** like XORing TRNG outputs and the critical role of random numbers in generating **secret cryptographic keys**.

---

## 📝 Summary
The questions cover four primary topics in Random Number Generation:

* **Randomness and Entropy Fundamentals**: The definition of random numbers as a uniform selection from a set, the distinction between objective Uniformity and subjective Predictability, and the use of Shannon's Entropy to measure the uncertainty or "surprise" in a sequence.
* **Generator Classifications (TRNG vs. PRNG)**: The operational differences between True Random Number Generators (TRNG), which rely on physical phenomena like thermal noise, and Pseudo-Random Number Generators (PRNG), which use deterministic algorithms initiated by a seed.
* **Algorithmic Implementations**: The mechanics of specific generators, including the Linear Congruential Generator (LCG) and Mersenne Twister (fast but cryptographically insecure), and the Blum Blum Shub algorithm (secure based on the difficulty of integer factorization).
* **Security Criteria and Validation**: The requirements for a Cryptographically Secure PRNG (CSPRNG), specifically the Next bit test and Forward security, and the application of statistical tests such as Frequency, Serial, Poker, and Autocorrelation tests to detect weaknesses.
