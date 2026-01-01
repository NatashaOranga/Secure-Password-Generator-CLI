# 🔐 Password Generator

**365 Days of Code - Day 1** 

A secure command-line password generator built with Python. Generate strong, customizable passwords for all your security needs.

## 🎯 Project Overview

This is my first project in my 365 Days of Code challenge! The goal is to code every day for a year and build a portfolio of projects.

**Day 1 Goal:** Build a practical CLI tool that I'll actually use.

## ✨ Features

- ✅ Generate passwords of any length
- ✅ Customize character types (uppercase, lowercase, numbers, special characters)
- ✅ Generate multiple passwords at once
- ✅ Avoid ambiguous characters (0, O, 1, l, I)
- ✅ Copy to clipboard support
- ✅ Cryptographically secure random generation
- ✅ Multiple convenience modes (PIN, alphanumeric, etc.)

## 🚀 Installation

### Prerequisites
- Python 3.6 or higher

### Optional Dependencies
For clipboard support:
```bash
pip install pyperclip
```

### Setup
```bash
# Clone the repository
git clone https://github.com/YOUR-USERNAME/password-generator.git
cd password-generator

# Make executable (Mac/Linux)
chmod +x password_gen.py
```

## 📖 Usage

### Basic Usage
```bash
# Generate a 16-character password (default)
python password_gen.py

# Generate a 20-character password
python password_gen.py -l 20

# Generate 5 passwords
python password_gen.py -l 16 -c 5
```

### Character Type Options
```bash
# No special characters
python password_gen.py --no-special

# Only lowercase letters
python password_gen.py --only-lower

# Only numbers (PIN mode)
python password_gen.py -l 6 --only-digits

# Alphanumeric only (no special characters)
python password_gen.py --only-alphanum
```

### Advanced Options
```bash
# Avoid ambiguous characters (0, O, 1, l, I)
python password_gen.py --avoid-ambiguous

# Copy to clipboard
python password_gen.py --copy

# Combine options
python password_gen.py -l 20 -c 3 --no-special --avoid-ambiguous
```

### All Options
```
-l, --length          Password length (default: 16)
-c, --count           Number of passwords to generate (default: 1)
--no-upper            Exclude uppercase letters
--no-lower            Exclude lowercase letters
--no-digits           Exclude numbers
--no-special          Exclude special characters
--only-lower          Only lowercase letters
--only-upper          Only uppercase letters
--only-digits         Only numbers (PIN mode)
--only-alphanum       Only letters and numbers
--avoid-ambiguous     Avoid ambiguous characters
--copy                Copy first password to clipboard
```

## 💡 Examples

```bash
# Strong password for a website
python password_gen.py -l 16

# WiFi password (no ambiguous characters)
python password_gen.py -l 24 --avoid-ambiguous

# PIN code
python password_gen.py -l 6 --only-digits

# Memorable password (lowercase + numbers only)
python password_gen.py -l 12 --only-lower --no-special

# Generate multiple options and copy the first
python password_gen.py -l 18 -c 5 --copy
```

## 🛠️ Technical Details

- Uses Python's `secrets` module for cryptographically secure random generation
- Falls back to `random` module if `secrets` is unavailable
- Comprehensive argument parsing with `argparse`
- Error handling for invalid inputs
- Cross-platform clipboard support (optional)

## 📝 What I Learned (Day 1)

- Command-line argument parsing with `argparse`
- Secure random generation in Python
- String manipulation and character pools
- Git basics (init, add, commit, push)
- Creating a practical, reusable tool

## 🔮 Future Enhancements

- [ ] Password strength indicator
- [ ] Passphrase generation (e.g., "correct-horse-battery-staple")
- [ ] Check against common password lists
- [ ] Save passwords to encrypted file
- [ ] Web interface version
- [ ] Bulk generation to file

## 📜 License

MIT License - feel free to use this for your own projects!

## 🤝 Contributing

This is a learning project, but suggestions and improvements are welcome! Feel free to:
- Open an issue
- Submit a pull request
- Share ideas for new features

## 🌟 365 Days of Code Challenge

Follow my journey as I code every day for a year! 

- **Day 1:** CLI Password Generator ✅
- **Day 2:** Coming soon...

Check out my [GitHub profile](https://github.com/NatashaOranga) for more projects!

## 📧 Contact

Have questions or suggestions? Feel free to reach out!

---

⭐ If you found this useful, give it a star!

**#365DaysOfCode** **#Day1** **#Python** **#CLI**
