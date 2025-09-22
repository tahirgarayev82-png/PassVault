# PassVault

---

## PassVault — Encrypted Password Vault**

```markdown
# PassVault

**PassVault** — a local encrypted password vault using a master password and KDF. Uses PBKDF2HMAC and Fernet encryption.

---

## ⚡ Features

- Initialize a local vault file
- Add, get, list, and delete passwords
- Master password with secure KDF (PBKDF2HMAC)
- All values encrypted with Fernet
- Secure local storage with recommended backups

---

## 🚀 Usage

```bash
# Initialize vault
python3 passvault.py init myvault.json

# Add a password
python3 passvault.py add myvault.json --name github

# Retrieve a password
python3 passvault.py get myvault.json --name github

# List all entries
python3 passvault.py list myvault.json

# Delete an entry
python3 passvault.py delete myvault.json --name github

---

## ⚙️ Configuration / Optional Modifications

Use a strong master password to unlock full access

Increase KDF iterations (iterations) in the JSON file for higher security

Extend functionality: CLI autofill, password generator, or external API integration

Important: Do not use a weak master password, as it compromises encryption security.

