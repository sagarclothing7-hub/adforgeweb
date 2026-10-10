# Deploying AdForgeAI to Netlify

Your project is already configured with `netlify.toml` and `public/_redirects` for 100% compatible Netlify deployment with client-side SPA routing.

---

### Method 1: Netlify Drop (Fastest — 10 seconds, No Code / No CLI)
1. In your project, run `npm run build` (or download the pre-built `dist/` folder).
2. Go to **[https://app.netlify.com/drop](https://app.netlify.com/drop)** in your browser.
3. Drag and drop the **`dist`** folder into the designated area on Netlify.
4. Your website is instantly live with a free SSL certificate and custom `.netlify.app` domain!

---

### Method 2: Git Repository (Recommended for Automatic Updates)
1. Push your repository to GitHub, GitLab, or Bitbucket.
2. Log in to [Netlify](https://app.netlify.com/) and click **"Add new site"** > **"Import an existing project"**.
3. Choose your Git provider and select this repository.
4. Netlify will auto-detect your configuration from `netlify.toml`:
   - **Build command:** `npm run build`
   - **Publish directory:** `dist`
5. Click **"Deploy site"**. Every future push to your Git branch will automatically rebuild and deploy!

---

### Method 3: Netlify CLI
1. Run in your terminal:
   ```bash
   npx netlify login
   ```
2. Deploy the built site:
   ```bash
   npm run build
   npx netlify deploy --prod --dir=dist
   ```
3. Follow the short on-screen prompts to select or create a site.

---

### Already Live in Google Cloud
Your application is also hosted directly on Google Cloud:
- **Shared App URL:** https://ais-pre-5acfkdb442rmpr66vpcqzk-302171267457.asia-southeast1.run.app
