# Secure QR Code Encryption System

## Project Overview

This project is a **client-side Secure QR Code Encryption System** developed as an individual academic project.  
The system allows users to **encrypt plaintext messages using a password**, convert the encrypted data into a **QR code**, and later **decrypt the QR code back into the original message** using the same password.

All encryption and decryption operations are performed **locally in the user’s web browser**, without using any backend server.

---

## Objectives

- Understand password-based encryption concepts
- Apply symmetric encryption (AES) in a practical application
- Demonstrate secure data storage using QR codes
- Develop a browser-based encryption system using JavaScript
- Ensure data privacy by performing all operations client-side

---

## Technologies Used

- **Programming Languages:**  
  - HTML  
  - CSS  
  - JavaScript

- **Cryptography:**  
  - Web Crypto API (AES encryption)

- **Libraries:**  
  - `QRCode.js` – QR code generation  
  - `jsQR` – QR code decoding from images

- **Hosting Platform:**  
  - GitHub Pages

---

## Project Structure
```
Secure-QR-Code-Encryption-System/
│
├── index.html          # Main web page
├── styles.css          # User interface styling
├── app.js              # Application logic
│
├── js/
│ ├── base64.js         # Base64/Base64URL encoding utilities
│ ├── password.js       # Password validation logic
│ ├── crypto.js         # AES encryption and decryption
│ ├── qr.js             # QR generation and decoding
│ └── ui.js             # User interface helpers
│
├── libs/
│ ├── qrcode.min.js     # QR code generation library
│ └── jsQR.js           # QR code decoding library
│
└── README.md           # Project documentation
```
---

## How the System Works

The encryption and decryption process follows this flow:

### Encryption
```
1. User enters a plaintext message.
2. User enters a password (minimum 12 characters).
3. The message is encrypted using AES.
4. The encrypted data is embedded into a QR code.
5. The QR code will be generate and can save as image.
```

### Decryption
```
1. User uploads the previously generated QR code image.
2. User enters the same password used during encryption.
3. The encrypted data is decrypted.
4. The original plaintext message is displayed.
```
---

## How to Run the Application

### Online (Recommended)
Visit the live demo hosted on GitHub Pages:
```
https://lykeosovann.github.io/Secure-QR-Code-Encryption-System/
```

### Locally
```
1. Download or clone the repository.
2. Open `index.html` in any modern web browser.
3. Ensure JavaScript is enabled.
```
```
No installation or server setup is required.
```
---

## Features
```
- Password-protected encryption
- QR code generation and scanning
- Client-side encryption and decryption
- No data storage or server communication
- Works entirely in the browser
```
---

## Security Notes
```
- Passwords are never stored or transmitted.
- All cryptographic operations occur locally in the browser.
- Using an incorrect password will result in failed decryption.
- The system is designed for educational purposes.
```
---

## Limitations
```
- QR codes must be downloaded as images (screenshots may reduce quality)
- No backend or key recovery mechanism
- Intended for learning and demonstration, not large-scale production use
```
---

## Future Goals
```
- Improve encryption by adding AES, RSA , SHA, etc.
- Adapt the system for CTF (Capture The Flag) challenge.
- Support firect QR code scanning on mobile devices.
```
## Author
```
**Ly keosovann**
Bachelor of Telecom and Networking
Specialization: Cybersecurity / Cryptography
```
