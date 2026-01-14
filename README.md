# Stone Lake Inn Website

A beautiful, rustic website for Stone Lake Inn - a bed & breakfast in the Pocono Mountains.

## Quick Start

Simply open `index.html` in a browser, or deploy to any static hosting service.

### Local Development
```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve

# Then open http://localhost:8000
```

## Project Structure

```
stonelake/
├── index.html          # Homepage
├── accommodations.html # Room listings & details
├── property.html       # Property amenities & gallery
├── things-to-do.html   # Local attractions & activities
├── book.html           # Booking inquiry form
├── about.html          # About & Contact page
├── css/
│   └── styles.css      # All styles (CSS custom properties)
├── js/
│   └── main.js         # Interactive features
└── images/             # All property photos
```

## Updating Content

### Adding/Changing Photos

1. Add new photos to the `images/` folder
2. Reference them in HTML: `<img src="images/your-photo.jpg" alt="Description">`
3. Recommended image sizes:
   - Hero images: 1920x1080px or larger
   - Room images: 1200x800px
   - Gallery thumbnails: 800x600px

### Current Image Placeholders

These images need to be added/replaced:
- `room-aviator.jpg` - The Aviator Room
- `room-aviator-2.jpg`, `room-aviator-3.jpg` - Aviator Room details
- `room-wine-2.jpg`, `room-wine-3.jpg` - Wine Room details
- `room-emerald-2.jpg`, `room-emerald-3.jpg` - Emerald Room details
- `room-loft-1.jpg`, `room-loft-2.jpg` - Third floor rooms
- `hot-tub.jpg` - Hot tub area
- `fire-pit.jpg` - Fire pit area
- `skydiving-view.jpg` - View of airport/skydiving
- `gallery-2.jpg` through `gallery-8.jpg` - Gallery images
- `activity-*.jpg` - Activity photos (skydiving, paintball, rafting, etc.)

### Changing Colors

Edit CSS custom properties in `css/styles.css`:

```css
:root {
  --burgundy: #722F37;      /* Primary color */
  --forest: #2D4A3E;        /* Secondary color */
  --cream: #F5F1EB;         /* Background */
  --charcoal: #2C2C2C;      /* Text */
  --gold: #B8860B;          /* Accents */
}
```

### Updating Contact Information

Search and replace these placeholders throughout the HTML files:
- `hello@stonelakeinn.com` - Email address
- `(570) 123-4567` - Phone number
- Formspree form ID in `book.html`

## Setting Up the Booking Form

The booking form is ready for [Formspree](https://formspree.io):

1. Create a free account at formspree.io
2. Create a new form
3. Copy your form endpoint (e.g., `https://formspree.io/f/xyzabc`)
4. In `book.html`, replace `YOUR_FORM_ID` in the form action:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```
5. Remove the JavaScript demo handler at the bottom of `book.html`

## Deployment Options

### Netlify (Recommended)
1. Push to GitHub
2. Connect repo to Netlify
3. Deploy automatically

### Vercel
1. Push to GitHub
2. Import project to Vercel
3. Deploy

### GitHub Pages
1. Push to GitHub
2. Enable Pages in repo settings
3. Select branch/folder

### Manual Upload
Upload all files to any web host that serves static files.

## Features

- **Responsive Design**: Works on all devices
- **Fast Loading**: No frameworks, pure HTML/CSS/JS
- **SEO Ready**: Semantic HTML, meta descriptions
- **Accessible**: Proper heading structure, alt text
- **Easy Updates**: Clear file structure, CSS variables
- **Interactive Elements**:
  - Scroll animations
  - Mobile navigation
  - FAQ accordion
  - Image lightbox gallery
  - Form validation

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Updating with AI

This site is designed to be easily updated using AI tools like Claude Code:

1. Describe what you want to change
2. AI can edit HTML content, CSS styles, or add new sections
3. Review changes before deploying

Example prompts:
- "Change the primary color to deep blue"
- "Add a new room called 'The Mountain Room'"
- "Update the check-in time to 4 PM"
- "Add a winter special banner to the homepage"

---

Built with care for Stone Lake Inn.
