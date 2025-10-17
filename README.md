# secure-dropbox
SecureDropBox — End-to-end encrypted file sharing web app with built-in threat modeling and attack simulations.

### 🧩 Project Overview

**SecureDropBox** provides a secure environment for file transfer between users using a hybrid encryption system.  
Each file is encrypted client-side with a symmetric AES-256 key, and that key is further encrypted using RSA or ECC public keys for each intended recipient.  
This ensures that only the intended receiver can decrypt and access the file.

The project also includes a **Threat Modeling** section built with OWASP Threat Dragon, using the **STRIDE** methodology to identify and mitigate potential threats like spoofing, tampering, information disclosure, and denial of service.

An optional **Attack Simulation Module** allows developers to visualize how end-to-end encryption prevents Man-in-the-Middle (MITM) and replay attacks in a controlled development environment.

---

### ✨ Key Features
- 🔐 **End-to-End Encryption (E2EE):** Hybrid RSA + AES encryption ensures complete privacy.
- 🧍‍♂️ **User Authentication:** Secure login with bcrypt/Argon2 password hashing and optional OAuth2 (Google/GitHub).
- 🧠 **Threat Modeling:** STRIDE-based threat analysis using OWASP Threat Dragon or Microsoft TMT.
- ⚔️ **Attack Simulation:** Educational MITM/replay attack visualization.
- 🗂️ **Secure File Storage:** Encrypted blobs stored in MongoDB or PostgreSQL.
- 🪵 **Audit Logging:** Optional cryptographically signed access logs.
- 🐳 **Containerized Deployment:** Docker setup for easy deployment to Heroku, Render, or AWS.

---

### 🧰 Tech Stack
**Frontend:** Next.js / React  
**Backend:** Node.js (Express)  
**Database:** MongoDB (with AES-encrypted data)  
**Encryption Libraries:** `crypto`, `openpgp.js`  
**Threat Modeling:** OWASP Threat Dragon  
**Deployment:** Docker + Heroku / Render / Vercel

---

### ⚠️ Disclaimer
This project is for **educational and demonstration purposes only**.  
Do not use in production environments without a full security audit.
