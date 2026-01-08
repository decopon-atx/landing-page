# Decopon Landing Page - Session Handoff

## Current State (Jan 7, 2026)

### What's Built
- **Animated hero video**: Felt decopon characters doing decoden craft (piping cream on phone case)
- **Full responsive landing page**: Mobile breakpoints at 480px/375px
- **"Meet the Founders" section**: Instagram embed of Tricia's interview (just added, not yet committed)
- **Email-only booking**: hello@decoponatx.com
- **Branding**: "Decopon" (not DecoponATX), white footer, no LinkedIn

### Key Files
- `~/Business/DecoponATX/landing_page/index.html` - Main page
- `felt_deco/hero-video.mp4` - Cropped hero video (watermark removed)
- `felt_deco/Felted_Fruit_World_Video_Generation/` - All Veo 3 video generations
- `decopon_brand_kit/` - Symlink to brand assets

### GitHub
- **Repo**: https://github.com/decopon-atx/landing-page
- **Auth**: Logged in as `decopon-atx` (not meeezus)
- **Status**: 2 commits pushed (mobile responsiveness + TopGolf $90+ pricing)
- **Pending**: Instagram embed section not yet committed

### Deployment
- **NOT using Vercel** - using FTP instead
- **Waiting on**: Tricia to provide FTP credentials
- **Live URL**: https://events.decoponatx.com/

### Veo 3.1 Prompt Template (SAVE THIS)
```json
{
  "prompt": "detailed 2-4 sentence description",
  "style": "aesthetic and technical approach",
  "camera_movement": "how camera moves",
  "lighting": "lighting setup",
  "duration": "8 seconds",
  "aspect_ratio": "16:9",
  "mood": "emotional tone",
  "additional_parameters": {
    "motion_intensity": "how much movement",
    "color_palette": "colors to use"
  }
}
```

### Prompts That Worked

**Felt characters doing decoden (hero video):**
```
Cozy needle-felted scene. Cute round orange felt citrus characters with tiny green leaves, dot eyes and sweet smiles gathered around a felt phone case. A hand pipes whipped cream onto the case while the orange characters watch with curiosity and excitement. Some characters peek from the sides, others lean in to watch. Felt strawberries and small charms on the case. Soft cream and tan felt background. Warm intimate crafting moment.
```

**Felt world landscape (first hero attempt):**
```
A cozy needle-felted miniature world. Cute round felt fruit characters with tiny leaves, simple dot eyes and small smiles - mostly orange, with a few yellow friends. Rolling soft felt hills in cream and warm caramel tones. Fluffy white felt clouds. One felt tree. Characters doing various activities - two chatting in foreground, one sitting under tree, one walking on distant hill. Warm studio lighting. Wide 16:9 landscape. Peaceful atmosphere. Smooth slow horizontal camera pan with parallax depth. Clear open center for text.
```

### Pending Tasks
1. [x] Commit Instagram embed to git
2. [x] Get FTP credentials from Tricia
3. [x] Deploy to live site via FTP
4. [x] Test Instagram embed works on live site
5. [x] Downloaded Instagram video via instaloader (self-hosted)

**All tasks complete! Site is live.**

### Page Flow (current)
1. Hero (felt video background + text overlay)
2. "See the Magic Happen" (workshop video placeholder)
3. "Meet the Founders" (Instagram embed - NEW)
4. Problem/Agitate section
5. Value stack
6. How it works
7. Gallery
8. Testimonials
9. Pricing ($750/10 people, $65 additional)
10. FAQ
11. Booking (email only)
12. Footer

### Quick Commands
```bash
# Check GitHub auth
gh auth status

# Push to GitHub
cd ~/Business/DecoponATX/landing_page && git add . && git commit -m "message" && git push

# Switch GitHub accounts
gh auth logout && gh auth login

# Open landing page locally
open ~/Business/DecoponATX/landing_page/index.html
```
