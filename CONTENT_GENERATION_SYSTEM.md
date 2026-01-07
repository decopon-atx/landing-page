# DecoponATX Content Generation System

## Overview

This system uses **Gemini Pro** with **Nano Banana** to generate on-brand felt/kawaii character assets for DecoponATX marketing materials.

## Tools Used

- **Gemini Pro** - Primary generation engine (via Google AI Studio or API)
- **Nano Banana** - Image generation model within Gemini
- **Ralph Plugin** (optional) - For automating batch content creation in Claude Code

---

## Asset Types Generated

### 1. Felt Character Scenes
- Decopon mascots in lifestyle settings
- Examples: "Soft. Sweet. Yours." landscape scene
- Use: Social media, hero sections, email headers

### 2. Phone Case Mockups
- Decoden-style phone cases with charms
- Examples: Bear + decopon case, Cinnamoroll + flowers case
- Use: Gallery section, product showcase, ads

### 3. Process/Workshop Imagery
- Characters demonstrating the creation process
- Examples: Whipped cream piping scene
- Use: How-it-works sections, tutorials, stories

### 4. Decorative Elements
- Circular frames, wreaths, borders
- Examples: Feltguys circular wreath
- Use: Footer, dividers, social profile pics

---

## Brand Guidelines for Generation

### Visual Style
- **Medium:** Needle felted / wool felt aesthetic
- **Characters:** Kawaii decopon (Japanese citrus) with faces
- **Colors:** Orange (#FFA85C), cream (#FFF8E8), green leaves, soft pastels
- **Texture:** Soft, fluffy, tactile wool appearance
- **Mood:** Warm, inviting, playful but professional

### Prompt Structure Template

```
[Scene/Subject] made of needle felt wool, kawaii style,
featuring decopon (Japanese orange) characters with cute faces,
soft pastel colors, cream and orange palette,
[additional elements],
soft lighting, warm atmosphere, high quality render
```

### Example Prompts

**Character Scene:**
```
A group of kawaii needle felt decopon characters with cute faces
having a picnic in a felt meadow, soft pastel colors,
cream and orange palette with green felt trees,
warm sunlight, cozy atmosphere, high quality render
```

**Phone Case Mockup:**
```
Flat lay photo of a decoden phone case with whipped cream texture,
decorated with kawaii needle felt decopon charms and small bears,
pearl beads, pastel flowers, orange and cream color scheme,
styled product photography, soft natural lighting
```

**Workshop Process:**
```
Needle felt kawaii characters watching someone pipe whipped cream
onto a phone case, workshop setting, felt texture on everything,
warm and inviting atmosphere, soft lighting,
cream and orange color palette
```

**Social Graphic:**
```
Circular wreath frame made of needle felt kawaii decopon characters
with cute faces, whipped cream swirls, macarons, hearts,
cream background, soft shadows, perfect for profile picture,
high quality render
```

---

## Workflow: Generating New Assets

### Step 1: Define the Asset Need
- What type? (scene, mockup, graphic, etc.)
- Where will it be used? (social, website, email, etc.)
- What size/format? (square, landscape, portrait)

### Step 2: Generate Prompt with Gemini Pro

Use this meta-prompt:
```
Create a Nano Banana prompt for a [ASSET TYPE] that:
- Features kawaii needle felt decopon characters
- Uses the DecoponATX brand palette (orange, cream, soft pastels)
- Conveys [EMOTION/MESSAGE]
- Will be used for [PLATFORM/PLACEMENT]

Follow the style of these existing assets: soft, warm, felt texture,
kawaii faces on characters, whipped cream textures where appropriate.
```

### Step 3: Generate in Gemini with Nano Banana
1. Open Google AI Studio (aistudio.google.com) or Gemini app
2. Select Nano Banana / image generation mode
3. Paste your prompt
4. Generate variations
5. Select best result
6. Download and save to `felt_deco/` folder

### Step 4: Post-Process (if needed)
- Crop/resize for platform requirements
- Add text overlays (use Fredoka font)
- Add Decopon logo badge if promotional

---

## Batch Generation with Ralph

For creating multiple assets at once, use the Ralph plugin:

```bash
/ralph-loop "Generate 5 social media graphics for DecoponATX using Gemini Pro prompts. For each:
1. Create a unique prompt following the brand guidelines
2. Save the prompt to a file
3. Log the generation task
<promise>ALL 5 PROMPTS COMPLETE</promise>" --max-iterations 10 --completion-promise "ALL 5 PROMPTS COMPLETE"
```

---

## Content Calendar Integration

### Weekly Social Content Needs
- **Monday:** Motivational/brand scene (1 image)
- **Wednesday:** Process/behind-scenes (1 image)
- **Friday:** Product showcase (1-2 images)
- **Stories:** 2-3 quick graphics per week

### Monthly Batch Generation
Generate 15-20 assets at start of month:
- 4 character scenes
- 4 phone case mockups
- 4 process images
- 4 decorative elements

---

## File Organization

```
landing_page/
└── felt_deco/
    ├── scenes/           # Character scenes and landscapes
    ├── mockups/          # Phone case product images
    ├── process/          # Workshop/creation imagery
    ├── graphics/         # Social graphics, frames, badges
    └── archive/          # Unused but saved generations
```

---

## Quality Checklist

Before using a generated asset:
- [ ] Characters look kawaii (cute faces, not creepy)
- [ ] Colors match brand palette
- [ ] Felt texture is visible and consistent
- [ ] No weird AI artifacts or distortions
- [ ] Appropriate resolution for intended use
- [ ] Consistent with existing brand imagery

---

## Current Asset Inventory

| File | Type | Best Use |
|------|------|----------|
| feltguys.png | Decorative frame | Footer, profile pic |
| image-76f6c3ae...jpeg | Brand scene | Hero, dividers |
| image-c896e04d...jpeg | Social graphic | Instagram, stories |
| feltvidscreenshot.png | Process | How-it-works |
| image-2a615214...png | Product mockup | Gallery, ads |
| image-e2b06b87...png | Product mockup | Gallery, showcase |
| animated-video-1765987490680.mov | Video | Social, hero |

---

## Tips for Best Results

1. **Be specific about felt texture** - Always mention "needle felt" or "wool felt"
2. **Include "kawaii" and "cute faces"** - Ensures friendly expressions
3. **Reference existing assets** - Maintain visual consistency
4. **Generate multiples** - Pick the best from variations
5. **Iterate on good prompts** - Save prompts that work well

---

## Gemini Pro System Prompt

Use this system prompt in Gemini for consistent brand output:

```
You are a creative director for DecoponATX, a kawaii phone case
decorating workshop brand. Generate images using Nano Banana that
produce on-brand felt character assets.

Brand essence: Soft, sweet, playful, warm, Japanese-inspired
Key character: Decopon (Japanese orange) with kawaii face
Textures: Needle felt wool, whipped cream, soft pastels
Colors: Orange #FFA85C, cream #FFF8E8, soft greens, pastels

Always produce images matching the existing brand aesthetic of
cozy, handmade, adorable visuals.
```

### Direct Generation in Gemini

Simply tell Gemini:
```
Generate a Nano Banana image of [description] in the DecoponATX
felt kawaii style - needle felt decopon characters, orange and
cream colors, soft warm lighting.
```

---

**Last Updated:** January 6, 2025
**Created By:** Claude Code Session
