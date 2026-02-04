# Warefor Hero Section - Odoo Website Snippet

A responsive hero section snippet for Odoo Website (16+) featuring a warehouse background with an overlay card.

## Files

- `wf_hero_snippet.xml` - QWeb template for the hero section
- `wf_hero_snippet.scss` - SCSS styles for assets_frontend

## Installation

1. Copy `wf_hero_snippet.xml` to your Odoo module's `views/` folder
2. Copy `wf_hero_snippet.scss` to `static/src/scss/`
3. Add the XML file to your `__manifest__.py` data list
4. Register the SCSS in assets_frontend in `__manifest__.py`:

```python
'assets': {
    'web.assets_frontend': [
        'your_module/static/src/scss/wf_hero_snippet.scss',
    ],
},
```

## Image

Add a background image at:
`/your_module/static/src/img/hero-warehouse.jpg`

## Features

- Responsive design (desktop, tablet, mobile)
- Bootstrap grid compatible
- Frosted glass card effect
- Hover animations on button
- All class names prefixed with `wf-` to avoid conflicts
