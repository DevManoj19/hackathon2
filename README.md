# 🏛️ Heritage Archive DID Verification System

A decentralized identity (DID) and verifiable credential system designed to register, verify, and archive heritage contributors using the W3C DID standard and `didkit`. This project enables secure, tamper-proof recognition of individuals contributing to cultural preservation efforts.

---

## ✨ Features

✅ **DID Generation** using Ed25519 cryptographic keys  
✅ **Verifiable Credentials** issuance & verification with `didkit`  
✅ **Metadata Registry** with timestamps and GDPR-style storage  
✅ **Contributor Onboarding Workflow** end-to-end  
✅ **Credential Signing** + export to JSON  
✅ **Credential Verification** (W3C-compliant)  
✅ **Dataverse API Integration** to fetch heritage dataset info  
✅ **System Backup** with JSON export  
✅ **Final Report Generator** for audit/documentation  
✅ **DID Validator** + QR code data stub (extensible)

---

## 🧪 Demo (Run in Jupyter Notebook or VS Code)

```bash
# Install dependencies first
pip install didkit pyld requests nest_asyncio
````

```python
# Jupyter-specific setup
import nest_asyncio
nest_asyncio.apply()

# Run main logic
await main()
```

### 🔍 Sample Output

* ✅ Generated DID: `did:key:z6Mk...`
* 🧾 Verifiable credential issued and verified
* 🗂️ Contributor metadata stored:

  ```json
  {
    "name": "Dr. Priya Sharma",
    "location": "Kolkata, West Bengal",
    "contribution_type": "Manuscript Digitization"
  }
  ```
* 💾 Credential saved as `heritage_credential_<workflow_id>.json`

---

## 📦 Project Structure

```
📁 heritage_did_system/
├── heritage_did_verifier.py         # Main logic
├── requirements.txt                 # All dependencies
├── README.md                        # You're reading this!
├── heritage_registry.json           # Exported metadata registry
├── heritage_credential_*.json      # Signed credential(s)
```

---

## 🛡️ Technologies Used

* [`didkit`](https://github.com/spruceid/didkit) — Verifiable Credential Toolkit
* `pyld` — JSON-LD processor
* `requests` — Dataverse API integration
* `nest_asyncio` — Async fix for Jupyter
* `uuid`, `json`, `datetime` — Core Python tools

---

## 🧠 Ideal Use Cases

* Cultural heritage institutions
* Academic digital humanities projects
* Historical document digitization projects
* Decentralized contributor tracking systems

---

## 📄 License

MIT License. Feel free to fork, contribute, or deploy.

---

## 💬 Contact

Developed with ❤️ by **[DevManoj19](https://github.com/DevManoj19)**
Drop feedback, issues, or collab ideas anytime!

---

## 📦setup.sh/requirements.txt

```txt
didkit
pyld
requests
nest_asyncio
````

> ✅ Make sure `libsodium` is installed via system package manager for `didkit`:

```bash
# Ubuntu/Debian
sudo apt-get install libsodium-dev

````
```bash
# macOS
brew install libsodium
```

---
