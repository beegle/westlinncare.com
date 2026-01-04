# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Single-page marketing website for West Linn Care, an adult foster home in West Linn, Oregon. Published on GitHub Pages at westlinncare.com.

## Development

**Local preview:** Open `index.html` directly in a browser (no build step required).

**Deployment:** Push to `main` branch - GitHub Pages auto-deploys.

## Technical Constraints

- **No external libraries** - native HTML, CSS, and JavaScript only
- **Single page** - all content on one scrollable page with anchor navigation
- **Relative paths** - all asset paths must be relative for GitHub Pages

## Content Workflow

Section content is drafted in `drafts/*.md` files. When converting to HTML:
1. Read the section markdown from drafts folder
2. Apply design guidelines below
3. Use semantic HTML (section, article, nav, etc.)
4. Insert into index.html at appropriate location

## Design System

### Color Palette (from logo)
| Role | Color | Usage |
|------|-------|-------|
| Primary Background | `#F5EDD8` | Main sections |
| Secondary Background | `#FFFFFF` | Alternating sections |
| Primary Text | `#5C4D42` | Body text, headings |
| Accent | `#B89A85` | Buttons, links |
| Accent Hover | `#9A7B68` | Interactive states |
| Border/Divider | `#E5DCC9` | Subtle separators |

### Typography
- System font stack (no external fonts)
- Serif or elegant sans-serif for headings
- Clean sans-serif for body

### Tone
- Warm and homey, not clinical
- Emphasize "home" over "facility"
- Simple design matching the line-art logo style

## Business Details
- **Name**: West Linn Care
- **Location**: West Linn, Oregon
- **Type**: Adult foster home for general aging care
- **Capacity**: Two homes, 5 residents each (10 total)
- **Second Home**: Opening Early 2025 (display as "Coming Soon")
- **Owners**: Ken Beegle and Cristina Beegle

## Page Sections (in order)

### 1. Header 
- Logo (images/logo.jpeg)
- "West Linn Care" text

### 2. Hero / Marketing Description
- Prominent tagline (placeholder - owner will finalize)
- Brief welcoming introduction
- Call-to-action button for tours
- Background could use hero image or soft gradient

### 3. About Adult Foster Homes
- Explanation of what an adult foster home is
- How it differs from larger facilities
- Benefits of smaller, home-based care

### 4. Services
Include these services:
- Meals (home-cooked)
- Medication management
- Activities and engagement
- Personal care assistance
- Housekeeping and laundry
- Companionship

**Do NOT include**: 24-hour care, memory care, transportation

### 5. Amenities
- Private rooms each with half bath
- Large outdoor space
- Home-like environment

### 6. Gallery
- Photo gallery section
- Placeholder images until real photos are provided
- See Photo TODO List below

### 7. Our Team (may be removed in final version)
- Ken Beegle - Owner/Licensor, years of experience
- Cristina Beegle - Owner/Licensor, years of experience
- Keep minimal

### 8. Second Home Announcement
- "Coming Soon - Early 2025"
- Brief mention of expanded capacity

### 9. Contact
- Phone number (placeholder until provided)
- Email address (placeholder until provided)
- Physical address (placeholder until provided)
- Tour request form (name, email, phone, preferred date, message)

### 10. Footer
- Copyright
- Basic links
- Location reference

## Photo TODO List

### Required Photos (dimensions and specs)
All photos should be:
- **Format**: JPG or WebP for photos, PNG for graphics
- **Resolution**: 72 DPI minimum for web (save originals at higher res)
- **Max file size**: Under 500KB each for performance

| Photo | Suggested Dimensions | Purpose |
|-------|---------------------|---------|
| Hero image | 1920x1080px | Main banner, exterior or welcoming interior |
| Exterior front (Home 1) | 1200x800px | Gallery, shows curb appeal |
| Exterior front (Home 2) | 1200x800px | Gallery, "Coming Soon" section |
| Common living area | 1200x800px | Gallery, shows homey atmosphere |
| Dining area | 1200x800px | Gallery, meal service |
| Sample bedroom | 1200x800px | Gallery, private room showcase |
| Sample bathroom | 800x600px | Gallery, half bath in rooms |
| Outdoor space | 1200x800px | Gallery, large yard/patio |
| Kitchen | 1200x800px | Gallery, home-cooked meals |
| Activity/sitting area | 1200x800px | Gallery, daily life |
| Ken Beegle headshot | 400x400px | Team section (square crop) |
| Cristina Beegle headshot | 400x400px | Team section (square crop) |

### Photo Guidelines
- Natural lighting preferred
- Rooms should be clean and staged
- No residents in photos (privacy)
- Capture warmth and comfort, avoid clinical feel
- Horizontal orientation for most shots

## Content Placeholders Needed
- [ ] Final tagline selection
- [ ] Ken's years of experience in care
- [ ] Cristina's years of experience in care
- [ ] Phone number
- [ ] Email address
- [ ] Physical address(es)
- [ ] Specific activity examples offered

## File Structure
```
/
├── index.html
├── styles.css
├── script.js
├── images/
│   ├── logo.jpeg
│   ├── hero.jpg
│   ├── gallery/
│   └── team/
├── CLAUDE.md
└── README.md
```

## GitHub Pages Notes
- Main branch deployment
- Custom domain configured via CNAME file
- Ensure all asset paths are relative

## Form Handling
Use **Formspree** for the tour request form.
- Free tier allows 50 submissions/month
- Form action: `https://formspree.io/f/{form_id}`
- Owner will need to create a Formspree account and provide the form ID
- Submissions are sent directly to the connected email address

### Form Fields
- Name (required)
- Email (required)
- Phone (optional)
- Preferred contact method (email/phone)
- Preferred tour date (optional)
- Message (optional)

### Setup Steps
1. Owner creates account at formspree.io
2. Creates new form, connects email
3. Provides form ID to add to the HTML form action
