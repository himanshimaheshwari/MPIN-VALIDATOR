# 🔐 MPIN Strength Validator

This project implements a complete **MPIN (Mobile Personal Identification Number) Validator** in Python. It detects weak 4-digit and 6-digit MPINs based on patterns, demographics (like DOB, spouse DOB, anniversary), and randomness (entropy). The logic is built step-by-step through multiple modules, all of which are included in this repository.

---

## ✅ Features

- **Pattern Detection**: Checks for:
  - Repeated digits (e.g., 1111, 2222)
  - Sequential digits (e.g., 1234, 4321)
  - Palindromes (e.g., 1221)
  - Common years (e.g., 1999, 2020)
  - Arithmetic progression
  - Mirror patterns, double-double, odd-even, etc.

- **Demographic Pattern Detection**:
  - Matches MPIN with DOB, Spouse DOB, and Anniversary
  - Extracts all relevant 4-digit or 6-digit combinations

- **Entropy-based Analysis** (for 6-digit MPINs):
  - Shannon entropy
  - Repeating subpatterns
  - Low uniqueness

- **Flexible PIN Length**: Handles both 4-digit and 6-digit PINs

- **Modular Code Design**:
  - `parta.py`: Basic validator
  - `partb.py`: Adds demographic support
  - `partc.py`: Logic-based extensions
  - `partd.py`: Entropy and pattern analysis for 6-digit MPINs
  - `parte.py`: Final validator with explanations and testing

---

## 📁 Files Included

- `parta.py` – Entry-level MPIN validator (4-digit)
- `partb.py` – Includes date-based demographic pattern matching
- `partc.py` – Expands pattern logic (e.g., mirror, arithmetic)
- `partd.py` – Advanced 6-digit MPIN checks including entropy
- `parte.py` – Final integration with all components and unit tests

---

## 🚀 Usage

1. Make sure you have **Python 3.7+** installed.

2. Run any script directly:

```bash
python parte.py
