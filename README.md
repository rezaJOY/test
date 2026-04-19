# GHOREO – Host Trust Landing Page

A responsive landing page for GHOREO, a platform for hosts in Dhaka to manage bookings, resolve disputes, and receive payouts.

**Live Site:** [ghoreo.com](https://ghoreo.com)

## Features

### Design & UX
- Responsive design for mobile, tablet, and desktop
- Security labels and verification badges
- Brand colors (teal #003C32, light gray #F7F7F7)
- Sticky call-to-action button linked to Google Form

### SEO & Social Optimization
- Meta tags for title, description, keywords, author, and geo-targeting (Dhaka)
- Open Graph image (1200x630) for Facebook, LinkedIn, Twitter, WhatsApp previews
- Twitter Card configuration for large image summaries
- Canonical URL to prevent duplicate content issues

### Progressive Web App
- Complete favicon set for desktop, iOS, and Android
- Web app manifest file (site.webmanifest)
- Theme color configuration for browser UI

## File Structure

```
.
|-- index.html
|-- site.webmanifest
|-- Og-image.jpg
|-- favicon-32x32.png
|-- favicon-16x16.png
|-- favicon.ico
|-- apple-touch-icon.png
|-- android-chrome-192x192.png
+-- android-chrome-512x512.png
```

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/rezaJOY/Ghoreo-host-trust.git
cd Ghoreo-host-trust
```

### 2. Customize Content

Edit `index.html` to update:

- **Lines 8-15:** Meta description and keywords
- **Lines 50-80:** Hero section text and value proposition
- **Line 120:** Google Form URL in CTA button
- **Lines 150-180:** Corporate info and contact details

### 3. Replace Social Image

Replace `Og-image.jpg` with your own 1200x630 social media preview image

### 4. Preview Locally

Open `index.html` in a browser to preview changes before deploying

## Deployment

### GitHub Pages (Current Setup)

This repository is deployed via GitHub Pages at [ghoreo.com](https://ghoreo.com).

**Every push to `main` branch automatically deploys to production.**

#### Initial Setup (Already Done)
1. Go to repository Settings -> Pages
2. Source: Deploy from branch `main`, folder `/` (root)
3. Custom domain: `ghoreo.com`
4. Enforce HTTPS: Enabled


#### Making Updates
1. Edit files directly on GitHub (click pencil icon) or push from local
2. Commit changes to `main` branch
3. Changes go live automatically in 30-60 seconds
4. Check deployment status: Settings -> Pages

### Alternative: Deploy to Another Host

If moving to a different hosting provider:

**Netlify:**
- Connect GitHub repo
- Build command: Leave empty
- Publish directory: `/`

**Cloudflare Pages:**
- Connect GitHub repo
- Framework preset: None
- Build command: Leave empty
- Build output directory: `/`

**Vercel:**
- Import GitHub repo
- Framework preset: Other
- Build settings: Default

## Verification & Testing

Before going live, test the following:

- **OG Image Preview:** [OpenGraph.xyz](https://www.opengraph.xyz/)
- **Facebook Sharing:** [Facebook Debugger](https://developers.facebook.com/tools/debug/)
- **Twitter Cards:** [Twitter Card Validator](https://cards-dev.twitter.com/validator)
- **Favicon Check:** Open DevTools (F12) -> Network tab -> reload -> verify all icons load (200 status)
- **Mobile Responsiveness:** Test on actual mobile devices or use browser DevTools
- **Form Submission:** Test the CTA button and Google Form integration

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom styling with media queries for responsive design
- **Vanilla JavaScript** - Minimal interactions (no frameworks)
- **Google Fonts** - Typography (if applicable)
- **Progressive Enhancement** - Works without JavaScript enabled

## Troubleshooting

### Site Not Updating After Push

1. Check GitHub Actions tab for deployment status
2. Hard refresh browser (Ctrl+F5 or Cmd+Shift+R)
3. Clear browser cache
4. Wait 2-3 minutes for CDN propagation

### Custom Domain Not Working

1. Verify DNS records at Namecheap (Advanced DNS)
2. Check GitHub Pages settings (Custom domain field should show green checkmark)
3. Wait 24-48 hours for DNS propagation (usually faster)
4. Use [DNS Checker](https://dnschecker.org) to verify propagation

### HTTPS Not Enabled

1. Ensure custom domain DNS is properly configured
2. Wait 10-30 minutes after DNS verification
3. Return to Settings -> Pages and enable "Enforce HTTPS"
4. If certificate provisioning fails, remove and re-add custom domain

### Favicon Not Showing

1. Clear browser cache completely
2. Check that all favicon files are in root directory
3. Verify `site.webmanifest` file is accessible
4. Test in incognito/private browsing mode

### Form Not Submitting

1. Verify Google Form link in CTA button is correct
2. Check that form is set to "Accept responses"
3. Test form link directly in new tab
4. Ensure form doesn't require sign-in

## Contact & Support

For questions or support:

- **Email:** info@ghoreo.com
- **Website:** https://ghoreo.com

## Contributing

This is a proprietary business repository. External contributions are not accepted. For GHOREO team members:

1. Create a feature branch from `main`
2. Make changes and test locally
3. Submit pull request with clear description
4. Get approval before merging to `main`

## License & Copyright

© 2024-2026 **M/s. GHOREO**. All rights reserved.

This repository is proprietary to GHOREO, a registered business entity operating under trade license in Dhaka, Bangladesh. 

Unauthorized copying, distribution, modification, or use of this code without written permission from GHOREO is strictly prohibited. This includes but is not limited to:

- Reproducing the code in any form
- Using the code for commercial purposes
- Creating derivative works
- Distributing the code to third parties

For licensing inquiries, contact: info@ghoreo.com

---

**Built with care by the GHOREO team** | Empowering hosts in Dhaka since 2026
