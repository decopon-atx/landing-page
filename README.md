# DecoponATX Landing Page

**Status:** Ready for hero video
**File:** `index.html` — Open in browser or deploy to web

---

## Quick Start

### 1. **Get the Video Ready**
Once Tricia delivers the hero video (60-90 seconds), you have 2 options:

**Option A: YouTube (Recommended - easiest)**
1. Upload video to YouTube (unlisted is fine)
2. Copy the YouTube video ID (from URL: youtube.com/watch?v=`VIDEO_ID`)
3. In `index.html`, find the commented YouTube embed (line ~200):
```html
<!-- OPTION A: YouTube Embed (uncomment when ready) -->
<iframe width="100%" height="600" src="https://www.youtube.com/embed/VIDEO_ID"
```
4. Replace `VIDEO_ID` with your actual ID
5. Delete the video placeholder div above it

**Option B: Direct File (File size matters)**
1. Save video file: `/Business/DecoponATX/landing_page/hero-video.mp4`
2. In `index.html`, uncomment the video tag (line ~206):
```html
<!-- OPTION B: Direct video file -->
<video controls>
    <source src="hero-video.mp4" type="video/mp4">
```
3. Delete the placeholder div

---

### 2. **Deploy to Web**

**Quick Hosting Option: Netlify (free)**
1. Go to netlify.com
2. Drag & drop the landing_page folder
3. Done. You have a live URL.

**Or: Use GitHub Pages**
1. Push folder to GitHub
2. Enable Pages in repo settings
3. Site goes live at `username.github.io/repo`

**Or: Your own server**
1. Upload `index.html` + `hero-video.mp4` to your server
2. Visit the URL

---

### 3. **Add Content ASAP**

**Gallery (photos):**
- Replace `[Case Design 1]`, `[Case Design 2]`, etc. with actual case photos
- Use high-quality images (1200x1200px minimum)
- Show finished cases + workshop moments

**Testimonials:**
- Uncomment these once you have them
- Include actual client names + titles

**Contact Form:**
- Current form just shows an alert
- Integration options:
  - **Calendly:** Replace form with Calendly embed
  - **Email:** Use Formspree.io (free)
  - **Zapier:** Capture forms → Google Sheets or email
  - **Custom:** If you have backend

---

## File Structure

```
landing_page/
├── index.html                          (Main landing page)
├── README.md                           (This file)
├── hero-video.mp4                      (ADD: Your video file)
├── landing_page_architecture.png       (Reference: page structure)
├── high_conversion_landing_page.jpeg   (Reference: design inspiration)
└── funnel_surfing_transcript.txt       (Reference: content ideas)
```

---

## Video Specs

**Ideal Hero Video:**
- **Length:** 60-90 seconds
- **Content:** Finished cases → process → experience → people's reactions → finished cases again
- **Format:** MP4 or upload to YouTube
- **Quality:** 1080p minimum (4K is great)
- **Audio:** Music or natural sound both work

**What Tricia should film:**
1. **Aesthetic (15 sec):** Showcase beautiful finished cases
2. **Process (30 sec):** Close-ups of cream piping, charm placement
3. **Experience (20 sec):** People creating, laughing, enjoying
4. **Outcome (15 sec):** Final cases being held, worn, shown off

---

## Email Capture Integration

**Current Setup:**
- Form placeholder (just shows alert)
- Ready for Calendly or email service integration

**To Enable Actual Emails:**

### Option 1: Calendly (Recommended for booking calls)
```html
<!-- Replace the email-form div with: -->
<div id="calendly-embed"></div>
<script type="text/javascript" src="https://assets.calendly.com/assets/external/widget.js"></script>
<script type="text/javascript">Calendly.initBadgeWidget({url: 'https://calendly.com/YOUR_PROFILE/discovery-call', text: 'Book a Call', color: '667eea'});</script>
```

### Option 2: Formspree (Email captures)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```
(Get form ID from formspree.io)

### Option 3: Google Sheets (Zapier)
1. Create Google Sheet with columns: Name, Email, Phone
2. Connect to Zapier
3. Set up: Form submission → Google Sheets row
4. Point form to Zapier webhook

---

## Tracking & Analytics

**To add Google Analytics:**
1. Get your GA tracking ID from google.com/analytics
2. Add this before `</head>`:
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_ID');
</script>
```

**Track:**
- Who visits the page
- Video play/watch time
- Form submissions
- Button clicks
- Scroll depth

---

## Design Notes

**Colors:**
- Primary: `#667eea` (purple-blue)
- Text: `#1a1a1a` (dark)
- Background: `#fafafa` (light gray)

**Change colors easily:**
- Find: `#667eea` in CSS
- Replace with your brand color

**Responsive:**
- Looks good on mobile, tablet, desktop
- Tested down to 320px width

---

## Next Steps

### Week 1 (When video is ready):
1. [ ] Get video from Tricia
2. [ ] Add to `index.html` (YouTube or file)
3. [ ] Deploy to Netlify or GitHub Pages
4. [ ] Test on mobile
5. [ ] Share link: `https://your-domain.com`

### Week 2 (When you have photos):
1. [ ] Add case photos to gallery
2. [ ] Add first testimonial
3. [ ] Set up email capture (Calendly/Formspree)
4. [ ] Add Google Analytics

### Week 3+:
1. [ ] Add more testimonials
2. [ ] Rotate gallery photos
3. [ ] Track metrics
4. [ ] Optimize based on what converts

---

## Questions?

**Video embed not showing?**
- Check YouTube video ID spelling
- Make sure iframe width/height are correct
- Try refreshing cache (Ctrl+Shift+R)

**Form not submitting?**
- Set up Calendly or Formspree account
- Replace form `action` attribute
- Test on mobile browsers

**Page looks weird?**
- Clear browser cache
- Try different browser
- Check phone size on mobile
- Make sure CSS loaded (check Elements inspector)

---

**Live URL (once deployed):** `[Add here once live]`

**Last Updated:** Jan 6, 2025
