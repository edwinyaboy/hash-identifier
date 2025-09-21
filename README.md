# 🔎 Hash Identifier

A lightweight web tool to **identify hash types** by analyzing their **length**, **character set**, and **prefix markers**.  
Perfect for developers, pentesters, and security researchers who need quick offline hash recognition.

---

## ✨ Features
- ✅ Detects common hash algorithms:
  - **MD5, SHA-1, SHA-224, SHA-256, SHA-384, SHA-512**
  - **RIPEMD-160, NTLM, LM, CRC32**
  - **bcrypt, scrypt, Argon2, PBKDF2**
  - And more!
- ✅ Pattern-based detection:
  - String **length** (e.g., 32, 40, 64, 128 chars)
  - **Character set** (hexadecimal, Base64)
  - **Prefix markers** (`$2b$`, `$argon2id$`, `$pbkdf2$`)
- ✅ Runs **100% client-side** (no server required)
- ✅ Lightweight, mobile-friendly design

---

## 🚀 How It Works
1. Paste your hash into the text box.  
2. Click **Identify**.  
3. The tool checks:
   - String **length**  
   - **Charset** used (hex vs. Base64)  
   - **Known prefixes** for salted hashes  
4. Displays the **most likely algorithm(s)**.  

---

## 📊 Examples

| **Input Hash**                                                                 | **Detected Type**     |
|--------------------------------------------------------------------------------|-----------------------|
| `5d41402abc4b2a76b9719d911017c592`                                             | MD5 / NTLM            |
| `40bd001563085fc35165329ea1ff5c5ecbdbbeef`                                     | SHA-1 / RIPEMD-160    |
| `2cf24dba5fb0a30e26e83b2ac5b9e29e1b161e5c1fa7425e73043362938b9824`             | SHA-256               |
| `$2b$12$KIX/3tN9qYfWfQ0EJ7uJ0e1gSlPrk5z6Y7Ff1JK4i6lF1x09jvC8W`                 | bcrypt (salted)       |
| `$argon2id$v=19$m=4096,t=3,p=1$w8h3V5...`                                      | Argon2 (salted)       |
| `$pbkdf2$1000$ZGF0YQ$k8h29f8fs...`                                             | PBKDF2 (salted)       |
| `03b3c3f0`                                                                     | CRC32                 |

---

## 🛠️ Tech Stack
- **HTML5**  
- **CSS3**  
- **Vanilla JavaScript**  

Everything runs **client-side**. No external libraries or servers required.

---

## 📥 Installation
Clone the repo and open `index.html` in your browser:

```bash
git clone https://github.com/yourusername/hash-identifier
cd hash-identifier
