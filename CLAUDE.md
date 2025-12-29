# West Linn Care - Website Project

## Project Overview
Single-page marketing website for West Linn Care, an adult foster home in West Linn, Oregon. The site will be published on GitHub Pages with the custom domain westlinncare.com.

## Technical Requirements
- **No external libraries**: Use only native HTML, CSS, and JavaScript
- **Hosting**: GitHub Pages
- **Domain**: westlinncare.com
- **Single page**: All content on one scrollable page with navigation anchors

## Business Details
- **Name**: West Linn Care
- **Location**: West Linn, Oregon
- **Type**: Adult foster home specializing in general aging care
- **Capacity**: Two neighboring homes, 5 residents each (10 total)
- **Second Home Status**: Opening Early 2025 (display as "Coming Soon")
- **Owners/Licensors**: Ken Beegle and Cristina Beegle

## Design Guidelines

### Color Palette (derived from logo)
Based on images/logo.jpeg:
- **Primary Background**: Soft cream `#F5EDD8` (logo background)
- **Secondary Background**: White `#FFFFFF` (alternating sections)
- **Primary Text**: Warm brown/taupe `#5C4D42` (logo lines)
- **Accent**: Muted rose `#B89A85` (logo heart)
- **Accent Hover**: Deeper rose `#9A7B68`
- **Light Border/Divider**: `#E5DCC9`

### Typography
- Use system font stack for performance
- Headings: Serif or elegant sans-serif feel
- Body: Clean, readable sans-serif

### Tone & Feel
- Warm and homey (not clinical or institutional)
- Emphasize "home" over "facility"
- Simple, clean design matching the line-art logo style
- Gentle curves and soft edges where appropriate

## Page Sections (in order)

### 1. Header / Navigation
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
