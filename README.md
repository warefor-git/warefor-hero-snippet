# Warefor Logistics Journey Section - Odoo Website Snippet

A responsive "Your Logistics Journey" section snippet for Odoo Website (16+) featuring a 3-step visual with images, progress indicators, and tags.

## Preview

This snippet displays:
- Section header with title and subtitle
- Step 1: Your Challenges - Image with badge, progress indicator, and challenge tags
- Step 2: We Handle Everything - Feature icons, marketplace tags, warehouse image
- Step 3: You Focus on Growth - Growth scale indicator, retail partnership tags

## Files

- `wf_journey_snippet.xml` - Step 1 section template
- `wf_journey_snippet.scss` - Step 1 styles
- `wf_journey_step2.xml` - Step 2 section template
- `wf_journey_step3.xml` - Step 3 section template
- `wf_journey_steps.scss` - Steps 2 & 3 shared styles

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
