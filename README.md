# CountWise LLC website

Premium static HTML/CSS/JavaScript website for **https://countwisellc.com**. No build tools, paid hosting, or API keys required.

## Preview locally

Open `index.html` in a browser or run `python -m http.server 8000` from this folder, then open `http://localhost:8000`.

## Publish on GitHub Pages (free)

1. Sign in to GitHub and create a new **public** repository named `countwise-website`. GitHub Pages on GitHub Free supports public repositories.
2. Upload **all files and folders in this ZIP** to the repository root, including `index.html`, `CNAME`, `.nojekyll`, and `assets/`. Commit to the `main` branch.
3. Open **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, `main`, and `/ (root)`. Save.
4. Under **Custom domain**, enter `countwisellc.com` and save. The included `CNAME` file contains the same domain.
5. In **GoDaddy → My Products → countwisellc.com → DNS → DNS Records**, update the website DNS to GitHub Pages. For the apex `@`, use these **four A records** (GitHub Pages published addresses):
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
   For `www`, use a **CNAME** pointing to `YOUR_GITHUB_USERNAME.github.io` (replace with your actual username; no `https://` or repository path).
6. Remove **conflicting old website A/AAAA/CNAME records** only after you have identified them. Do **not** remove email MX/TXT records, nameservers, or unrelated records. Back up existing DNS first.
7. Allow DNS propagation. In GitHub **Settings → Pages**, wait until **Enforce HTTPS** is available and enable it. Verify both `https://countwisellc.com` and `https://www.countwisellc.com` redirect/resolve correctly.
8. Test the navigation and inquiry form on mobile and desktop.

**Important:** Changing DNS will replace the currently hosted GoDaddy website at this domain. Keep your GoDaddy website as a backup until the new one is tested. Domain registration stays with GoDaddy.

## Contact form

The contact form uses `mailto:`. It opens the visitor's configured email application with a prefilled message; **it does not automatically submit**. Visitors without an email application can use the visible Gmail address or phone number. For a hosted form later, choose a reputable form provider and update the privacy notice.
