# Aankda Landing Page

Coming soon landing page for [aankda.com](https://aankda.com).

## Deployment (GitHub Pages)

1. Create a new GitHub repository named `aankda-landing` (or any name)

2. Push this code:
   ```bash
   cd aankda-landing
   git init
   git add .
   git commit -m "Initial landing page"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/aankda-landing.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to repository Settings > Pages
   - Source: Deploy from a branch
   - Branch: main, folder: / (root)
   - Click Save

4. Configure DNS at your domain registrar:

   **Option A: Apex domain (aankda.com)**
   Add these A records:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

   **Option B: www subdomain (www.aankda.com)**
   Add a CNAME record:
   ```
   www -> YOUR_USERNAME.github.io
   ```

5. Wait for DNS propagation (can take up to 48 hours, usually faster)

6. In GitHub Pages settings, check "Enforce HTTPS" once the domain is verified

## Email Collection

Currently, the form just shows a success message. To actually collect emails, integrate with:
- Google Sheets (via Google Apps Script)
- Mailchimp
- ConvertKit
- Buttondown

## Local Development

Just open `index.html` in a browser.
