# Hosting Guide for Demo Shop

Built with WebSorted AI Website Builder

---

## Your Site is Live!

Your website is hosted on GitHub Pages at:
**https://arzcakes.github.io/test-shop/**

It may take 1-2 minutes for the first deployment to go live.

---

## Adding a Custom Domain

Want your site at **mybusiness.com** instead? Follow these steps:

### Step 1: Buy a Domain
Purchase a domain from any registrar:
- [Namecheap](https://www.namecheap.com) (recommended)
- [Google Domains](https://domains.google)
- [GoDaddy](https://www.godaddy.com)
- [Cloudflare](https://www.cloudflare.com/products/registrar/)

### Step 2: Configure DNS at Your Registrar
Log into your domain registrar's dashboard and add these DNS records:

**For www.yourdomain.com (CNAME record):**
| Type  | Name | Value                      |
|-------|------|----------------------------|
| CNAME | www  | arzcakes.github.io |

**For yourdomain.com (apex domain - A records):**
| Type | Name | Value           |
|------|------|-----------------|
| A    | @    | 185.199.108.153 |
| A    | @    | 185.199.109.153 |
| A    | @    | 185.199.110.153 |
| A    | @    | 185.199.111.153 |

### Step 3: Tell GitHub About Your Domain
1. Go to your repository: https://github.com/arzcakes/test-shop
2. Click **Settings** > **Pages**
3. Under "Custom domain", enter your domain (e.g., `www.mybusiness.com`)
4. Check **Enforce HTTPS** (free SSL certificate via Let's Encrypt)

### Step 4: Wait for DNS Propagation
DNS changes can take 5 minutes to 48 hours (usually under 30 minutes).
Check status at: https://dnschecker.org

---

## Pushing Updates

When you update your site in WebSorted, simply click **Deploy to GitHub** again.
Your changes will go live automatically within 1-2 minutes.

---

## Alternative Hosting Options

### Netlify (Free)
1. Go to [netlify.com](https://www.netlify.com) and sign up
2. Drag and drop your site files (index.html + styles.css) onto the deploy area
3. Your site is live instantly with a .netlify.app URL
4. Add a custom domain in Site Settings > Domain management

### Vercel (Free)
1. Go to [vercel.com](https://vercel.com) and sign up with GitHub
2. Import your repository
3. Vercel auto-deploys and gives you a .vercel.app URL
4. Add custom domains in Project Settings > Domains

### Traditional Web Hosting (cPanel/FTP)
1. Log into your hosting control panel
2. Navigate to File Manager or use an FTP client (e.g., FileZilla)
3. Upload index.html and styles.css to the public_html folder
4. Your site is live at your hosting domain

---

## Troubleshooting

**Site not loading?**
- Wait 1-2 minutes after deployment
- Check that GitHub Pages is enabled in repo Settings > Pages

**Custom domain not working?**
- Verify DNS records are correct at your registrar
- Wait up to 30 minutes for DNS propagation
- Ensure CNAME file exists in your repository

**HTTPS not working?**
- GitHub auto-provisions SSL via Let's Encrypt
- It can take up to 24 hours after DNS propagation
- Make sure "Enforce HTTPS" is checked in GitHub Pages settings

---

Need help? Visit [WebSorted Support](https://websorted.uk/support)
