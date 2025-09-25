
# 🚀 PET STORE API Bruno Collection

![Bruno Logo](https://docs.usebruno.com/img/bruno-logo.png)

This repository contains a Bruno collection for PET Store PET, STORE and USER flows across QA and PERF environments.

## 📁 Folder Structure

```text
bruno/
├── collection.bru
├── bruno.json
├── README.md
├── results.html
├── environments/
│   ├── PERF.bru
│   └── QA.bru
├── pet-store-suite/
│   ├── bruno.json
│   └── PET/
│       ├── CreatePet.bru
```

## 🧩 API Suite Overview

Below is a summary of all APIs available in this suite:


> 📝 **Note:** The above table is based on folder and file names. For exact payloads and headers, refer to the `.bru` files in each folder.

## 🖼️ Example Bruno Suite Screenshot

![Suite Screenshot](https://docs.usebruno.com/img/bruno-collection.png)

## 🛠️ Quick Start

1. Copy `.env.example` to `.env` and populate values:
  - `QA_X_API_KEY`
  - `PERF_X_API_KEY`
2. Open collection in Bruno and select the appropriate environment.

## 🚦 Running the Suite (CLI)

```bash
npm i -g @usebruno/cli
bru run --env-file "environments/QA.bru"
bru run --env-file "environments/PERF.bru"
```

## 🔒 Security
- Do not commit tokens or secrets. Secrets are loaded via dotenv and repository secrets in CI.
- Tokens are acquired using client credentials and stored as runtime vars only.
- `.gitignore` excludes `.env` and transient files.

## 📚 References
- [Bruno Documentation](https://docs.usebruno.com/)

