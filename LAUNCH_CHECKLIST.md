# DecoponATX Landing Page - Launch Checklist

## Pre-Launch (Do These First)

### Critical Path Items
- [ ] **Get hero video filmed** (60-90 seconds)
  - Structure: Aesthetic → Process → Experience → Results
  - Can be shot on iPhone with good lighting
  - Music or natural sound both work

- [ ] **Upload video to YouTube**
  - Can be "Unlisted" (not public, but shareable)
  - Copy the video ID from the URL
  - Example: `youtube.com/watch?v=dQw4w9WgXcQ` → ID is `dQw4w9WgXcQ`

- [ ] **Add video to landing page**
  - Open `index.html`
  - Find line 527 (YouTube embed option)
  - Replace `VIDEO_ID` with your actual ID
  - Delete the placeholder div above it (lines 521-525)

- [ ] **Set up Calendly account**
  - Go to calendly.com (free account works)
  - Create "Discovery Call" event type (15 minutes)
  - Copy your Calendly username
  - Choose integration option in `index.html` (line 804 or 812)
  - Replace `YOUR_CALENDLY_USERNAME` with your actual username

- [ ] **Update contact info**
  - Line 816: Update email address if different from `contact@decoponatx.com`
  - Line 826: Add your phone number (or remove if not ready for calls)
  - Line 842-843: Update footer email/phone

---

## Launch Day (30 minutes total)

### Deploy the Site
- [ ] **Option A: Netlify (Recommended - 5 min)**
  1. Go to netlify.com
  2. Sign up (free)
  3. Drag & drop the `landing_page` folder
  4. Get your live URL (e.g., `decoponatx.netlify.app`)
  5. Optional: Add custom domain later

- [ ] **Option B: GitHub Pages (10 min)**
  1. Create GitHub repo
  2. Push `landing_page` folder to repo
  3. Enable Pages in repo settings
  4. Live at `username.github.io/repo-name`

- [ ] **Option C: Your Own Hosting**
  - Upload `index.html` to your server
  - Make sure path is correct

### Test the Live Site
- [ ] **Desktop Testing**
  - Open in Chrome, Firefox, Safari
  - Click all CTAs (should scroll or link properly)
  - Test Calendly booking flow
  - Verify video plays

- [ ] **Mobile Testing**
  - Test on iPhone (Safari)
  - Test on Android (Chrome)
  - Verify video autoplays (muted)
  - Check all sections display correctly
  - Test booking flow on mobile

### Analytics Setup (Optional but Recommended)
- [ ] **Google Analytics 4**
  1. Go to analytics.google.com
  2. Create account/property
  3. Get tracking ID (starts with `G-`)
  4. Add to `index.html` line 863
  5. Uncomment GA code (lines 862-869)
  6. Verify tracking in GA dashboard (24hr delay)

---

## Week 1: First Marketing Push

### Share the Link
- [ ] **Warm Network (Day 1)**
  - Text 20 contacts: "Just launched my new workshop business. Would love your feedback: [LINK]"
  - Don't ask for bookings yet, just feedback

- [ ] **LinkedIn (Day 2-3)**
  - Update LinkedIn headline to include DecoponATX
  - Post about launch with link
  - Start sending video DMs (per business plan strategy)

- [ ] **Networking Events (Week 1)**
  - Attend 2 events with your phone case
  - Follow up with landing page link within 24 hours

- [ ] **Social Media (Day 1)**
  - Update Instagram bio with link
  - Post story about launch
  - Update TikTok bio with link

### Track Performance
- [ ] **Monitor Daily (First Week)**
  - Google Analytics: Traffic sources
  - Calendly: Booking conversion rate
  - Note: Which channel drives most traffic?
  - Note: Where are people dropping off?

---

## After First Event (Week 2-4)

### Content Updates
- [ ] **Gallery Photos**
  - Take 50+ photos at first event
  - Select best 6-8 for gallery
  - Replace placeholders (lines 646-681 in index.html)
  - Use high-quality, well-lit images

- [ ] **Testimonials**
  - Send follow-up email 2 days after event
  - Ask for testimonial (provide 3 questions)
  - Replace placeholder testimonials (lines 696-707)
  - Use real names + titles with permission

- [ ] **Video Enhancement**
  - Capture 3-5 video clips from event
  - Consider editing into hero video v2
  - Add "as seen in" social proof if applicable

### Optimization
- [ ] **Review Analytics (Week 4)**
  - What's the bounce rate?
  - Which CTA gets most clicks?
  - Mobile vs desktop conversion?
  - Adjust based on data

- [ ] **A/B Test Ideas**
  - Test headline variations
  - Test CTA button text
  - Test pricing display
  - Use Google Optimize (free)

---

## Month 2: Scale & Iterate

### Advanced Tracking
- [ ] **Set up event tracking**
  - Video play events
  - Scroll depth tracking
  - CTA click events
  - Form submissions

### SEO Optimization
- [ ] **Local SEO**
  - Google Business Profile
  - Yelp listing
  - Austin business directories
  - Get backlinks from Austin sites

### Social Proof Expansion
- [ ] **Add more testimonials** (aim for 5-7 total)
- [ ] **Add client logos** (if applicable)
- [ ] **Add "as featured in"** (if you get press)
- [ ] **Add workshop count** ("50+ workshops completed")

### Conversion Optimization
- [ ] **Exit-intent popup** (offer discount for first booking?)
- [ ] **Live chat widget** (if getting enough traffic)
- [ ] **FAQ expansion** (add questions from discovery calls)
- [ ] **Add video testimonials** (more powerful than text)

---

## Common Issues & Fixes

### Video won't play on mobile
- **Fix:** Use `playsinline` attribute in video tag
- **Check:** Video format (MP4 H.264 works best)
- **Check:** File size (compress to < 50MB for fast loading)

### Calendly not showing up
- **Fix:** Check JavaScript console for errors
- **Fix:** Verify Calendly username is correct
- **Fix:** Make sure script tag is included

### Page loads slowly
- **Fix:** Compress hero video
- **Fix:** Optimize images (use TinyPNG or similar)
- **Fix:** Consider lazy-loading images

### Mobile layout looks weird
- **Fix:** Test on actual devices, not just browser resize
- **Fix:** Check that viewport meta tag is present (line 5)
- **Fix:** Verify responsive CSS is working (@media queries)

### Not getting traffic
- **Fix:** Share link in 3+ channels per day
- **Fix:** Post content that links back to landing page
- **Fix:** Add link to email signature
- **Fix:** Run LinkedIn ads (Week 4+ if budget allows)

### Getting traffic but no bookings
- **Fix:** Review video (is it compelling?)
- **Fix:** Review pricing (is there sticker shock?)
- **Fix:** Add urgency ("Limited spots for January")
- **Fix:** Simplify CTA ("Book Free Call" not "Discovery Call")

---

## Metrics That Matter (Per Business Plan)

### Week 1-4 Focus:
- **Page visits:** 100+ in first month
- **Video play rate:** >50% of visitors
- **Scroll to booking:** >30% reach bottom
- **Discovery calls booked:** 8-12 from all channels

### Month 2-3 Focus:
- **Traffic sources:** Which channel has best conversion?
- **Cost per call:** Time invested / calls booked
- **Call-to-booking rate:** >40% close rate on calls
- **Testimonial collection:** 1 per event minimum

---

## Quick Wins

### Do These for Immediate Impact:

1. **Add your face to the page**
   - People buy from people
   - Add founder photo to "About" section
   - Or add to testimonials as "facilitator"

2. **Add urgency**
   - "Only 3 spots left in January"
   - "Next available: [DATE]"
   - "Book by [DATE] for early-bird pricing"

3. **Simplify the CTA**
   - Change "Book a Discovery Call" to "Book Free Call"
   - Or "Check Availability"
   - Or "Schedule a Workshop"

4. **Add social proof numbers**
   - "50+ workshops completed" (update as you go)
   - "500+ happy customers"
   - "4.9/5 rating on Google"

5. **Create scarcity**
   - "Only serving 10 clients this month"
   - "Limited to Austin metro area"
   - "Booking 4-6 weeks out"

---

## Success Metrics by Timeline

### Week 1 Success:
- ✅ Site is live and bug-free
- ✅ Shared with 20+ warm contacts
- ✅ 2-3 discovery calls booked
- ✅ Analytics tracking working

### Month 1 Success:
- ✅ 100+ page visits
- ✅ 8-12 discovery calls
- ✅ 3-4 workshops booked
- ✅ $2,500+ revenue
- ✅ First testimonials collected

### Month 3 Success:
- ✅ 500+ page visits
- ✅ 20+ discovery calls
- ✅ 10-12 workshops completed
- ✅ 5+ testimonials on page
- ✅ $8,000+ cumulative revenue

---

## Final Pre-Launch Check

Before you share the link publicly:

- [ ] Hero video is live and plays correctly
- [ ] Calendly booking works (test it yourself)
- [ ] All links work (test every button)
- [ ] Mobile version looks good (test on real phone)
- [ ] Contact info is correct
- [ ] No typos in headline/copy
- [ ] Analytics is tracking
- [ ] Site loads fast (<3 seconds)
- [ ] You've tested the full booking flow

**When all boxes are checked → YOU'RE READY TO LAUNCH!**

---

## Emergency Contacts

If something breaks and you need help:

1. **Video issues:** Re-upload to YouTube, check embed code
2. **Calendly issues:** Check Calendly help docs
3. **Hosting issues:** Check Netlify/GitHub status pages
4. **Analytics issues:** Check GA setup guide

---

**Remember:** Done is better than perfect. Launch with hero video + Calendly, iterate based on data.

Your landing page will improve with every workshop you run.

**Action: Set a launch date. Stick to it. Ship it.**
