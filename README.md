# GIGO Data, Inc. – Email & Domain Trust Infrastructure

This public repository contains the domain trust stack used by **GIGO Data, Inc.** for:

- 💌 **Email deliverability & authentication**
- 🔐 **Public trust disclosures**
- 🎨 **Brand-reinforced inbox identity (BIMI)**
- 📄 **Compliance with modern sending policies and protocols**

---

## 📁 Repository Contents

| File / Directory              | Purpose |
|------------------------------|---------|
| `.well-known/mta-sts.txt`    | Enforces STARTTLS for secure inbound mail |
| `.well-known/security.txt`   | Public security contact and policy notice |
| `gigo_logo_bimi.svg`         | Verified BIMI logo for inbox display |
| `index.html`                 | Redirects root domain to `www.gigodata.com` |
| `CNAME`                      | Maps GitHub Pages to custom domain |
| `.gitignore`                 | Professional-grade Git hygiene |
| `README.md`                  | This file — full trust stack overview |

---

## 🌐 GitHub Pages Deployment

Hosted at:  
👉 `https://www.gigodata.com`  
Root redirects:  
👉 `https://gigodata.com`

GitHub Pages is enabled using the `main` branch with root deployment. SSL is auto-issued via GitHub. DNS is routed through Cloudflare.

---

## ✅ Live Hosted Assets

All required files are publicly accessible over HTTPS:

- `https://gigodata.com/.well-known/security.txt`
- `https://mta-sts.gigodata.com/.well-known/mta-sts.txt`
- `https://gigodata.com/gigo_logo_bimi.svg`

---

## 🔐 Email Authentication

Configured for maximum deliverability and protection:

| Protocol | Status | Value |
|----------|--------|--------|
| SPF      | ✅ Valid | `v=spf1 include:_spf.google.com ~all` |
| DKIM     | ✅ Valid | Google Workspace keys |
| DMARC    | ✅ Quarantine | Reports to `dmarc@gigodata.com` |
| BIMI     | ✅ Logo published | See `default._bimi TXT` |
| TLS-RPT  | ✅ Enabled | Receives failure reports |
| MTA-STS  | ✅ Enforced | With max-age + full MX list |

---

## 📬 Email Domain Reputation

📊 You may monitor this domain’s inbox display and compliance using:

- [Gmail Postmaster Tools](https://postmaster.google.com/)
- [URIports Email Tools](https://uriports.com/tools)

---

## 🧠 About GIGO Data, Inc.

We believe in zero garbage in — and zero garbage out.  
GIGO Data< Inc. is an an ethical data ecosystem powered by trust, transparency, and open infrastructure.  
This repository reflects our commitment to technical integrity from Day 1.

---
