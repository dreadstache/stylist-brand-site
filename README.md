# Personal Brand Site

An interview-ready, single-page personal brand site. It needs no build step, framework, database, or account besides GitHub.

## Before publishing (five minutes)

1. Open `index.html` in a text editor.
2. Replace every `Your Name` / `YOUR NAME` with the preferred name.
3. Replace `hello@yourdomain.com` with a real email address.
4. Optionally edit the closing paragraph and credentials if a detail needs to be more specific.
5. Double-click `index.html` to preview it in a browser.

## Publish with GitHub Pages

1. Create a new GitHub repository, such as `yourname-style`.
2. Upload `index.html` and `styles.css` from this folder to the repository root (not inside another folder).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, then choose `main` and `/ (root)`, and save.
5. GitHub will provide an address like `https://username.github.io/yourname-style/` within a few minutes.

### Connect an existing custom domain

1. In **Settings → Pages**, enter the domain in **Custom domain** and save.
2. At the domain provider, follow the DNS values GitHub displays. For a `www` subdomain this is usually a CNAME record pointing to `username.github.io`.
3. Wait for GitHub to verify the domain, then enable **Enforce HTTPS**.

The current Google Sites page can remain online until the custom domain verification completes, then point the domain DNS to GitHub Pages. This avoids a blank-page intermission—the internet's least glamorous magic trick.

## Google Sites option

Google Sites cannot host this custom HTML/CSS as a real site; it only supports an embedded page. If you must keep Google Sites as the main address, publish this site through GitHub Pages and use **Insert → Embed → By URL** in Google Sites. Direct GitHub Pages is the better interview-day choice: it is faster, cleaner, and looks intentional.
