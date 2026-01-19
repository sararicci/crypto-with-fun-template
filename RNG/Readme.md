# Random Number Generator Comparison Exercise

## 📚 Overview

This repository contains an **in-class exercise** designed to help students understand the differences between various types of random number generators (RNGs) through hands-on experimentation and visual analysis.

**Duration:** 10–15 minutes  
**Level:** Introductory Cryptography / Computer Security

## 🎯 Learning Objectives

By the end of this exercise, students will be able to:

- Distinguish between True RNGs, Pseudo RNGs, and Cryptographically Secure PRNGs
- Generate random bit sequences using different methods
- Perform basic visual randomness tests
- Understand the security implications of using different RNG types in cryptographic applications

## 📂 Contents

- **`rng_exercise_slides.pdf`** - LaTeX Beamer presentation for classroom use
- **`rng_exercise_slides.tex`** - LaTeX source file
- **`sequences/`** - Folder for storing generated bit sequences (create during exercise)

## 🔧 Exercise Structure

### Part 1: Generate Three Sequences

Students will generate three 100-bit sequences using:

1. **True Random Number Generator (TRNG)**
   - Uses atmospheric noise from [random.org](https://www.random.org/integers/)
   - Represents genuine physical randomness

2. **Linear Congruential Generator (LCG)**
   - Deterministic algorithm commonly found in older programming languages
   - Fast but predictable and unsuitable for security

3. **Cryptographically Secure PRNG (CSPRNG)**
   - Uses Python's `secrets` module
   - Designed for cryptographic applications

### Part 2: Visual Analysis

Students perform simple tests:
- Count the ratio of 0s to 1s
- Look for patterns or repetitive sequences
- Identify which sequences "look" more random
- Discuss findings with peers

## 🚀 Quick Start Guide

### For Instructors

1. **Before Class:**
   - Review the slides (`rng_exercise_slides.pdf`)
   - Ensure students have access to Python (for LCG and CSPRNG generation)
   - Test the random.org link

2. **During Class:**
   - Present the slides (5 minutes)
   - Guide students through sequence generation (5–7 minutes)
   - Facilitate discussion on visual analysis (3–5 minutes)

3. **After Class:**
   - Optional: Have students run statistical tests on their sequences
   - Discussion forum: Share interesting findings

### For Students

#### Step 1: Generate True Random Sequence

1. Visit: **[https://www.random.org/integers/](https://www.random.org/integers/)**
2. Set parameters:
   - **Number of integers:** 100
   - **Min:** 0
   - **Max:** 1
   - **Format:** One column
3. Click "Get Numbers"
4. Save as `trng_sequence.txt`

#### Step 2: Generate LCG Sequence

Run this Python code:

```python
# Linear Congruential Generator
a, c, m = 1103515245, 12345, 2**31
seed = 42
sequence = []

for _ in range(100):
    seed = (a * seed + c) % m
    sequence.append(seed % 2)

print(''.join(map(str, sequence)))
```

Save output as `lcg_sequence.txt`

#### Step 3: Generate CSPRNG Sequence

Run this Python code:

```python
import secrets

sequence = [secrets.randbelow(2) for _ in range(100)]
print(''.join(map(str, sequence)))
```

Save output as `csprng_sequence.txt`

#### Step 4: Analyze

- Count 0s and 1s in each sequence
- Look for patterns (long runs, repetitions)
- Compare: Which looks most random? Why?

## 💡 Discussion Points

- **Can you visually tell the sequences apart?**
- **What makes something "look random"?**
- **Why is visual inspection insufficient for cryptographic purposes?**
- **When would you use each type of generator?**
- **What are the risks of using weak RNGs in security applications?**

## 🔗 Resources

- [Random.org](https://www.random.org/) - True random number service
- [NIST SP 800-90A](https://csrc.nist.gov/publications/detail/sp/800-90a/rev-1/final) - Recommendation for Random Number Generation
- [Python secrets module](https://docs.python.org/3/library/secrets.html) - Cryptographically strong random numbers

## 📝 Additional Activities

### Advanced Exercise
Run statistical tests using Python:

```python
from scipy.stats import chisquare

# Count 0s and 1s
counts = [sequence.count('0'), sequence.count('1')]
expected = [50, 50]

# Chi-square test
chi2, p_value = chisquare(counts, expected)
print(f"Chi-square: {chi2:.4f}, p-value: {p_value:.4f}")
```

### Homework Assignment
- Generate longer sequences (1000+ bits)
- Implement runs test
- Research the NIST randomness test suite
- Write a short report comparing the three generators

## 📄 License

This educational material is provided under the MIT License. Feel free to use and adapt for your courses.

## 🤝 Contributing

Found an error or have suggestions? Please open an issue or submit a pull request!

---

**Happy exploring randomness! 🎲**
