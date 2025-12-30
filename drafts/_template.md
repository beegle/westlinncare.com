# Section Draft Template

Use this format for all section drafts. When ready, provide the markdown file to Claude.ai and ask it to convert to HTML following the project's design guidelines.

---

## Standard Format

```markdown
# Section Name
<!-- section-id: kebab-case-id -->
<!-- status: draft | review | approved -->
<!-- last-updated: YYYY-MM-DD -->

## Content

[Main content goes here in markdown format]

## Notes for Conversion

- [Any specific styling notes]
- [Layout preferences]
- [Special considerations]

## Placeholders

- [ ] List any placeholder content that needs final values

## Approved By

- [ ] Content reviewed
- [ ] Ready for HTML conversion
```

---

## Conversion Instructions for Claude.ai

When converting a section draft to HTML:

1. **Read the section markdown file** from the drafts folder
2. **Follow design guidelines** from CLAUDE.md:
   - Primary Background: `#F5EDD8`
   - Secondary Background: `#FFFFFF`
   - Primary Text: `#5C4D42`
   - Accent: `#B89A85`
   - Accent Hover: `#9A7B68`
   - Light Border: `#E5DCC9`
3. **Use the section-id** as the HTML section's id attribute
4. **Apply consistent spacing** and responsive design
5. **Use semantic HTML** (section, article, nav, etc.)
6. **Insert into index.html** at the appropriate location
