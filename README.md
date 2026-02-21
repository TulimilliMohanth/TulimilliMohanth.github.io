# TulimilliMohanth.github.io / mohanth.me

This repository is the **user GitHub Pages** repo for the account `TulimilliMohanth`.

- **GitHub Pages URL**: `https://tulimillimohanth.github.io/`
- **Custom domain**: `https://mohanth.me/`

## Why `mohanth.me` shows “There isn't a GitHub Pages site here”

That specific 404 page appears when your domain resolves to GitHub Pages IPs, but **GitHub Pages does not have your custom domain connected to a Pages site** yet.

## Fix checklist

### 1) DNS records (at your domain provider)

For the apex/root domain `mohanth.me`, set **A** records to GitHub Pages:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

Optional but recommended (IPv6):

- `2606:50c0:8000::153`
- `2606:50c0:8001::153`
- `2606:50c0:8002::153`
- `2606:50c0:8003::153`

If you also want `www.mohanth.me`, set:

- `www` **CNAME** → `tulimillimohanth.github.io`

### 2) GitHub Pages settings (in this repo)

In GitHub: **Settings → Pages**

- **Custom domain**: set to `mohanth.me`
- Wait for **“DNS check successful”**
- Enable **“Enforce HTTPS”** (certificate issuance can take a bit after DNS is verified)

### 3) Ensure the site has an entry page

This repo includes `index.html`, so the site has a real homepage once Pages rebuilds.