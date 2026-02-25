MinKYC — Privacy-Preserving KYC on Solana

⚠️ READ-ONLY REPOSITORY ⚠️
Do not make manual commits to this repository. This repository is an automated deployment window. It is automatically updated and maintained by the MinKYC OSINT Bot pipeline. Any manual changes made here will be overwritten.

Production Website: https://getoutofthatgarden.github.io/minkyc-website/

Main Project Source Code: https://github.com/GetOutOfThatGarden/MinKYC

About MinKYC

MinKYC enables platforms to verify users meet regulatory requirements (age, residency, etc.) without storing sensitive identity data. This eliminates GDPR liability, reduces breach risk, and maintains full audit compliance.

The Automated OSINT Blog

In addition to the main marketing site, this domain hosts the MinKYC Intelligence Feed. An autonomous AI agent monitors global news for centralized KYC data breaches, generates intelligence reports, and publishes them directly to this website under /breaches/[company_slug].html.

Architecture & DevOps Stack

This repository serves as the public-facing display for a decoupled, modern CI/CD architecture:

Frontend Framework: React + TypeScript + Vite

Styling: Tailwind CSS v3

Hosting: GitHub Pages

CMS / Deployment Engine: Python + GitHub Actions + Gemini 2.5 AI

How Updates Work

The raw React source code lives in the MinKYC repository.

The compiled assets and HTML template are stored in a private automation repository (kyc-breach-bot).

When the AI agent detects a KYC breach, it generates a new HTML report, wraps it in the MinKYC UI template, and uses an SSH Deploy Key to push the entire website directly to this repository.

GitHub Pages detects the push and instantly updates the live website.

Related Links

Resource

URL

Live Site

https://getoutofthatgarden.github.io/minkyc-website/

Main Project Repo

https://github.com/GetOutOfThatGarden/MinKYC

Colosseum Hackathon

https://colosseum.com/agent-hackathon/projects/minkyc-e5qc5l

Demo Video

https://www.loom.com/share/9dced184732f48e0b754a2ad7c822687

Smart Contract

Explorer Link

Twitter/X Agent

@NH32WEB

License & Contact

License: MIT License — See main MinKYC repository for details.

Creator: @NH32WEB

Project Issues: GitHub Issues Tracker

Built with React, Tailwind CSS, and managed by AI.
