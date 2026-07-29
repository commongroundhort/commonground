# Common Ground Horticulture website

This folder contains a mobile-friendly single-page website for:

https://commongroundhorticulture.com.au

## Before publishing

Open `index.html` and replace:

- `0400000000`
- `0400 000 000`
- `hello@commongroundhorticulture.com.au`

with Melissa's real contact details.

You can also replace the two Unsplash image URLs in `styles.css` with your own photos later.

## Free publishing option: GitHub Pages

1. Create a GitHub account.
2. Create a new public repository named `commongroundhorticulture`.
3. Upload `index.html` and `styles.css`.
4. In the repository, open **Settings > Pages**.
5. Under **Build and deployment**, select:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /root
6. Save and wait for the GitHub Pages address to appear.
7. Add a file named `CNAME` containing:
   commongroundhorticulture.com.au
8. In Cloudflare DNS, point the domain to GitHub Pages.

## Cloudflare DNS for GitHub Pages

For the root domain, add these four A records:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

Add a CNAME record:

- Name: www
- Target: YOUR-GITHUB-USERNAME.github.io

Use DNS only initially if GitHub has trouble verifying the domain. After the custom domain is working, Cloudflare proxy can usually be turned back on.

## QR code

Point the QR code to:

https://commongroundhorticulture.com.au
