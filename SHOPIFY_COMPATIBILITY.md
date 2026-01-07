# Shopify Compatibility & Integration Options

**Last Updated:** January 5, 2025

---

## TL;DR: Is This Compatible with Shopify?

**Short answer:** No, not directly.

**Long answer:** This is a standalone HTML landing page. Your Shopify site uses different technology (Liquid templating, theme structure). But you have several options below.

---

## Current Setup

### Your Retail Site (decoponatx.com)
- **Platform:** Shopify
- **Purpose:** E-commerce (sell kits, charms, supplies)
- **Audience:** DIY craft enthusiasts, individual consumers
- **Tech:** Liquid templates, Shopify theme architecture
- **Font:** Quicksand
- **Colors:** Cream (#fff8f0), burnt orange (#ffa94d), deep blue (#135090)

### This B2B Landing Page
- **Platform:** Standalone HTML file
- **Purpose:** Corporate workshop bookings
- **Audience:** Austin HR managers, team leads
- **Tech:** Pure HTML/CSS (no framework)
- **Font:** Fredoka (from brand kit)
- **Colors:** Peachy orange (#FFA85C), dark brown (#4A2417), cream (#FFF8E8)

---

## Integration Options

### ✅ Option 1: Keep Separate (RECOMMENDED)

**Setup:**
- Retail site: decoponatx.com (Shopify)
- B2B landing page: corporate.decoponatx.com (Netlify/Vercel/custom hosting)

**Advantages:**
- ✅ Clean separation of audiences
- ✅ Different conversion funnels
- ✅ Easy to optimize each independently
- ✅ No technical conflicts
- ✅ Can use different domains or subdomains
- ✅ Track analytics separately

**Disadvantages:**
- ❌ Two sites to maintain
- ❌ Need separate hosting for landing page

**Cost:**
- Netlify: FREE (with custom domain option)
- Vercel: FREE (with custom domain option)
- Domain: ~$15/year if using subdomain

**How to implement:**
1. Deploy this landing page to Netlify (drag & drop folder)
2. Get free subdomain: `decoponatx-corporate.netlify.app`
3. OR add custom subdomain: `corporate.decoponatx.com`
4. Update DNS settings to point subdomain to Netlify
5. Done!

---

### ⚠️ Option 2: Embed in Shopify

**Setup:**
Create a new Shopify page with this HTML embedded as content

**Advantages:**
- ✅ Everything under one domain
- ✅ Use Shopify's hosting
- ✅ Single admin dashboard

**Disadvantages:**
- ❌ Shopify will add theme header/footer (conflicts with design)
- ❌ Limited customization without theme editing
- ❌ Performance overhead from Shopify framework
- ❌ May break some CSS/animations
- ❌ Harder to A/B test

**How to implement:**
1. Shopify Admin → Online Store → Pages → Add page
2. Click "Show HTML" in editor
3. Paste the HTML from index.html
4. Create custom template to hide theme elements
5. Assign page to custom template

**Technical challenges:**
- CSS conflicts with theme styles
- JavaScript conflicts
- Header/footer removal requires theme editing
- Mobile responsiveness might break

---

### 🛠️ Option 3: Rebuild as Shopify Section

**Setup:**
Convert this landing page to a Shopify custom section with Liquid syntax

**Advantages:**
- ✅ Native Shopify integration
- ✅ Can use Shopify's tools (analytics, CRM, etc.)
- ✅ Single platform

**Disadvantages:**
- ❌ Requires significant development time
- ❌ Need Liquid/Shopify expertise
- ❌ Harder to update/iterate
- ❌ Limited by Shopify's section architecture
- ❌ May require paid Shopify theme or custom development

**Effort required:**
- 8-12 hours of development
- Knowledge of Liquid templating
- Theme customization skills

**Not recommended unless:**
- You already have Shopify dev skills
- You want everything in one platform
- You have budget for custom development

---

## Recommended Path Forward

### For Your Situation:

**Use Option 1 (Separate Sites)** because:

1. **Different audiences:** Retail customers ≠ corporate buyers
2. **Different conversion goals:** E-commerce checkout ≠ discovery calls
3. **Speed to launch:** Deploy to Netlify in 5 minutes
4. **Flexibility:** Optimize B2B landing page without affecting retail sales
5. **Cost:** FREE hosting with Netlify
6. **Simplicity:** No Shopify theme conflicts

### Setup Steps (15 minutes):

1. **Deploy to Netlify:**
   - Go to netlify.com
   - Sign up (free)
   - Drag `landing_page` folder
   - Get URL: `decoponatx-corporate.netlify.app`

2. **Add Custom Subdomain (Optional):**
   - In Netlify: Settings → Domain Management → Add custom domain
   - Enter: `corporate.decoponatx.com`
   - Netlify gives you DNS records
   - Add CNAME record in your domain registrar
   - Wait 24-48 hours for DNS propagation

3. **Link from Retail Site:**
   - Add "Corporate Workshops" link to decoponatx.com navigation
   - Points to `corporate.decoponatx.com`

---

## Design Elements to Keep from Shopify Site

Based on decoponatx.com analysis:

### Already Incorporated:
- ✅ Fredoka font (from brand kit)
- ✅ Peachy orange color (#FFA85C - close to #ffa94d)
- ✅ Cream background (#FFF8E8 - close to #fff8f0)
- ✅ Sticky header
- ✅ Centered hero text
- ✅ CTA buttons with orange accent

### Could Add from Shopify Site:
1. **Quicksand font option** - Keep Fredoka or offer toggle?
2. **Deep blue accent** (#135090) - Could use for trust badges
3. **Generous padding** (40-60px) - Already using similar spacing
4. **Minimal shadows** - Could reduce shadow intensity
5. **Grid spacing** (8px desktop, 4px mobile) - Verify consistency

### Differences (Intentional for B2B):
- **B2B:** More structured, conversion-focused
- **Retail:** Playful, product-focused browsing
- **B2B:** Single CTA journey (book discovery call)
- **Retail:** Multiple products, add-to-cart flow

---

## Domain Strategy Options

### Option A: Subdomain
- **B2B:** corporate.decoponatx.com
- **Retail:** decoponatx.com
- **Cost:** Free (uses existing domain)

### Option B: Separate Domain
- **B2B:** decoponatxworkshops.com
- **Retail:** decoponatx.com
- **Cost:** ~$15/year for new domain

### Option C: Path-based
- **B2B:** decoponatx.com/corporate-workshops
- **Retail:** decoponatx.com
- **Note:** Requires Option 2 (embed in Shopify) or custom server config

**Recommendation:** Option A (subdomain) - Clean, professional, free

---

## FAQ

### Can I sell workshop bookings through Shopify?
**Yes, but not recommended.** Shopify is built for physical products, not service bookings. Better to use:
- Calendly (free, easy discovery calls)
- Stripe (direct payment processing)
- Shopify only if you want gift certificates or package sales

### Will this affect my Shopify SEO?
**No.** Separate domains/subdomains don't hurt each other. In fact, having a B2B subdomain can help:
- Target different keywords (corporate team building vs craft supplies)
- Different audiences won't confuse search engines
- Can rank for both commercial and retail queries

### Can I share customers between sites?
**Technically yes, but complicated.** Would require:
- Custom CRM integration
- Email list syncing
- Privacy compliance (GDPR, CCPA)
- Not necessary for launch

### What about email marketing?
**Keep separate lists:**
- Retail list: Craft enthusiasts, DIY hobbyists
- B2B list: HR managers, event planners
- Different messaging, different campaigns
- Can use same email service (Klaviyo, Mailchimp, etc.)

---

## Hosting Comparison

| Feature | Netlify (Recommended) | Vercel | Shopify Page | Custom Server |
|---------|----------------------|--------|--------------|---------------|
| **Cost** | FREE | FREE | Included | $5-20/mo |
| **Setup Time** | 5 min | 5 min | 30 min | 1-2 hours |
| **Custom Domain** | ✅ Free SSL | ✅ Free SSL | ✅ Via Shopify | ✅ Via DNS |
| **Conflicts** | None | None | Theme conflicts | None |
| **Performance** | Excellent | Excellent | Good | Varies |
| **Ease of Updates** | Drag & drop | Git push | Edit in Shopify | FTP/SSH |

---

## Migration Path (If You Want Shopify Later)

If you start with Netlify and later want to move to Shopify:

1. Keep landing page on Netlify (free)
2. Add booking products to Shopify (gift certificates, packages)
3. Link landing page → Shopify checkout for payments
4. Keep discovery calls on Calendly
5. Best of both worlds: Fast landing page + Shopify payment processing

---

## Action Items

### To Launch on Netlify (Do This):
1. [ ] Go to netlify.com and sign up
2. [ ] Drag `landing_page` folder to Netlify
3. [ ] Get your URL: `decoponatx-corporate.netlify.app`
4. [ ] Add hero video
5. [ ] Add Calendly username
6. [ ] Test on mobile
7. [ ] Share link!

### To Add Custom Subdomain (Optional):
1. [ ] In Netlify: Add `corporate.decoponatx.com`
2. [ ] Copy CNAME record from Netlify
3. [ ] Add CNAME to your domain registrar (wherever you bought decoponatx.com)
4. [ ] Wait 24-48 hours for DNS
5. [ ] SSL automatically activates

### To Link from Shopify Site (After Launch):
1. [ ] Shopify Admin → Navigation → Main menu
2. [ ] Add link: "Corporate Workshops"
3. [ ] URL: `https://corporate.decoponatx.com`
4. [ ] Save

---

## Bottom Line

**Don't try to force this into Shopify.**

**Why:**
- Different purposes (retail vs B2B)
- Different audiences
- Free hosting available
- Faster, cleaner, more flexible

**Deploy to Netlify in 5 minutes, launch, and start booking workshops.**

You can always integrate payment processing later if needed, but for discovery calls → workshops, this standalone approach is perfect.

---

**Questions?** Check the LAUNCH_CHECKLIST.md for deployment steps.
