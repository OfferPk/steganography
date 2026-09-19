# Steganography

Client-side tools for **image steganography** (LSB message hiding) and related local HTML demos. All processing runs in the browser; nothing is uploaded to a server.

## Contents

| File | Description |
|------|-------------|
| [`index.html`](index.html) | Main steganography app — hide/extract text in images (LSB, optional XOR/AES-style options) |
| `ssn-generator1.html` | Standalone SSN demo UI (v1) |
| `ssn-generator3.html` | Standalone SSN demo UI (v3) |
| `ssn-generator4.html` | Standalone SSN demo UI (v4) |
| `ssn-genrator5.html` | Standalone SSN demo UI (v5; legacy filename typo preserved) |
| `ssngenerator.html` | Earlier standalone SSN demo UI |

Exact duplicate copies of the v1 generator were removed in this cleanup (`ssn-generator2.html`, `ssn-genrator6.html`).

## Quick start (steganography)

1. Open `index.html` in a modern browser (or serve the folder with any static file server).
2. Upload a **PNG** image (preferred; JPEG compression can corrupt hidden data).
3. Enter a message, choose LSB mode / channel / encryption options, then **Hide Text** or **Extract Text**.

Optional: AES/DES/3DES options in the UI expect [CryptoJS](https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto-js.min.js) (already referenced from a CDN in `index.html`).

### Steganography features

- LSB embedding (1 / 2 / 4 bit)
- Channel selection (RGB or single channel)
- Optional simple XOR or CryptoJS-backed ciphers (some options are placeholders)
- Capacity hint based on image size and settings
- Local-only processing

## SSN demo pages

> **Disclaimer:** The SSN HTML pages are for educational / UI demonstration only. Generating or using fake Social Security Numbers for fraud or other unlawful activity is illegal. Do not use these demos for unlawful purposes.

These pages are standalone static demos (localStorage, UI polish). This repository cleanup does **not** change their behavior or add new generation features.

## Project layout

```
.
├── README.md
├── .gitignore
├── index.html              # steganography app
├── ssngenerator.html
├── ssn-generator1.html
├── ssn-generator3.html
├── ssn-generator4.html
└── ssn-genrator5.html
```

No build step or package manager is required — plain HTML/CSS/JS.

## License / use

Use responsibly and in accordance with applicable law. Prefer educational and personal experimentation only.
