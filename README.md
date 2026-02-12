# MinKYC Website

The official marketing website for **MinKYC** — a privacy-preserving KYC solution built on Solana.

**Live Site:** https://deeppink-wolverine-734172.hostingersite.com  
**Project:** https://colosseum.com/agent-hackathon/projects/minkyc-e5qc5l  
**Source Code:** https://github.com/GetOutOfThatGarden/MinKYC

---

## About MinKYC

MinKYC enables platforms to verify users meet regulatory requirements (age, residency, etc.) without storing sensitive identity data. This eliminates GDPR liability, reduces breach risk, and maintains full audit compliance.

### Key Benefits
- ✅ **No identity data stored** — Only cryptographic commitments touch the blockchain
- ✅ **GDPR compliant by design** — No honeypot of passport scans or ID documents
- ✅ **Immutable audit trail** — Every verification creates an on-chain receipt
- ✅ **Three-role workflow** — User, Platform, and Regulator each have distinct responsibilities

---

## Tech Stack

- **Framework:** React + TypeScript + Vite
- **Styling:** Tailwind CSS v3
- **Build Output:** Static HTML/CSS/JS
- **Hosting:** Hostinger Website Plan
- **Deployment:** GitHub → Hostinger auto-deploy

---

## Project Structure

```
/
├── index.html          # Main HTML entry point
├── assets/             # Bundled CSS and JS files
│   ├── index-*.css     # Tailwind styles
│   └── index-*.js      # React application bundle
├── vite.svg            # Favicon
└── README.md           # This file
```

---

## Development

### Local Development

```bash
# Clone the main MinKYC repo for source code
git clone https://github.com/GetOutOfThatGarden/MinKYC.git
cd MinKYC/minkyc-website

# Install dependencies
npm install

# Run dev server
npm run dev

# Build for production
npm run build
```

### Building from Source

The source code for this website is in the main MinKYC repository:
- **Source:** `/minkyc-website/` in the main repo
- **Build output:** `dist/` folder (this is what gets deployed)

---

## Deployment

This repository contains the **built static files** (not the source). Deployment is handled automatically by Hostinger.

### Manual Update Process

If you need to update the website:

1. Build the site from the main MinKYC repo:
   ```bash
   cd /path/to/MinKYC/minkyc-website
   npm run build
   ```

2. Copy the new `dist/` contents to this repo:
   ```bash
   cp -r /path/to/MinKYC/minkyc-website/dist/* /path/to/minkyc-website/
   ```

3. Commit and push:
   ```bash
   cd /path/to/minkyc-website
   git add -A
   git commit -m "Update website - [date/description]"
   git push origin main
   ```

4. Hostinger will auto-deploy from GitHub

---

## Related Links

| Resource | URL |
|----------|-----|
| **Main Project Repo** | https://github.com/GetOutOfThatGarden/MinKYC |
| **Colosseum Hackathon** | https://colosseum.com/agent-hackathon/projects/minkyc-e5qc5l |
| **Demo Video** | https://www.loom.com/share/9dced184732f48e0b754a2ad7c822687 |
| **Smart Contract** | https://explorer.solana.com/address/9zzT4KdUh7TEtiR8ioTMhDLWDa4c6ymzAjQsYYfvc3h1?cluster=devnet |
| **Twitter/X** | https://twitter.com/NH32WEB |

---

## Architecture Overview

```
┌─────────┐    ┌──────────┐    ┌──────────┐
│  USER   │───→│ PLATFORM │───→│  SOLANA  │
│ (local) │    │ (verify) │    │ (receipt)│
└─────────┘    └──────────┘    └──────────┘
     │                │                │
     ▼                ▼                ▼
Creates identity   Verifies      Immutable
+ commitment       proofs        audit trail
```

1. **User** creates identity locally (passport scan never leaves device)
2. **Platform** requests verification (e.g., "is this user over 18?")
3. **Solana** records the verification receipt on-chain

---

## Colosseum Agent Hackathon

This project was built for the **Colosseum Agent Hackathon** by:
- **Agent:** Bella-MinKYC-v2
- **Creator:** @NH32WEB
- **Status:** Submitted

---

## License

MIT License — See main MinKYC repository for details.

---

## Contact

- **Twitter:** @NH32WEB
- **Project Issues:** https://github.com/GetOutOfThatGarden/MinKYC/issues

---

*Built with React, Tailwind CSS, and deployed on Hostinger.*
