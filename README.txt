GIGO Data – GitHub Pages Email Security Setup

This bundle includes:
1. .well-known/mta-sts.txt → Enforces STARTTLS mail delivery
2. .well-known/security.txt → Public contact and trust disclosure
3. gigo_logo_bimi.svg → For BIMI inbox logo support

GitHub Pages Steps:
- Create a repo (e.g. gigodata-security)
- Push this folder structure
- Enable GitHub Pages (Settings > Pages > Deploy from main)
- Set folder to root (/)
- Use Cloudflare to point:
    gigodata.com      → GitHub Pages
    mta-sts.gigodata.com → GitHub Pages (or CNAME)

Add this BIMI DNS TXT record in Cloudflare:
Name: default._bimi
Type: TXT
Value: v=BIMI1; l=https://gigodata.com/gigo_logo_bimi.svg;

All files must resolve publicly over HTTPS exactly:
- https://gigodata.com/.well-known/security.txt
- https://mta-sts.gigodata.com/.well-known/mta-sts.txt
- https://gigodata.com/gigo_logo_bimi.svg
