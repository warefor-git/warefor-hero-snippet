# Warefor Logistics Journey Section - Odoo Website Snippet

A responsive "Your Logistics Journey" section snippet for Odoo Website (16+) featuring a step-by-step visual with image, progress indicator, and tags.

## Preview

This snippet displays:
- Section header with title and subtitle
- Step 1: Image with badge, icon + title, description, progress indicator, and challenge tags

## Files

- `wf_journey_snippet.xml` - QWeb template for the journey section
- `wf_journey_snippet.scss` - SCSS styles for assets_frontend

## Installation

1. Copy `wf_journey_snippet.xml` to your Odoo module's `views/` folder
2. Copy `wf_journey_snippet.scss` to `static/src/scss/`
3. Add the XML file to your `__manifest__.py` data list
4. Register the SCSS in assets_frontend in `__manifest__.py`:

```python
'assets': {
    'web.assets_frontend': [
        'your_module/static/src/scss/wf_journey_snippet.scss',
    ],
},
```

## Required Image

Add a background image at:
`/your_module/static/src/img/journey-ship.jpg`

## Features

- Responsive design (desktop, tablet, mobile)
- Bootstrap grid compatible (container, row, col)
- Progress indicator with icons
- Pill-style tags
- All class names prefixed with `wf-journey-` to avoid conflicts
- Font Awesome icons (fa-box, fa-clock, fa-cube, fa-check)

## Customization

### Modify Colors
Edit the SCSS variables:
- Primary: `#1a365d`
- Accent: `#c9a227`
- Gray: `#64748b`
- Background: `#f8f7f5`

### Add More Steps
Duplicate the `.wf-journey-step` row and update:
- Badge text (Step 2, Step 3)
- Image source
- Title and description
- Tags
