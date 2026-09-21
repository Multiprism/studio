# Video game studio website

A studio website inspired by the *structure and design principles* of strong independent game-studio sites: artwork-forward pages, concise studio copy, visible team members, clear projects, and a modern but playful visual system.

## Included

- `index.html` — full-screen art-led home page
- `projects.html` — project portfolio
- `team.html` — team grid and culture section
- `about.html` — studio story and behind-the-scenes gallery
- `contact.html` — contact routing and front-end form UI
- `styles.css` — full responsive design system
- `script.js` — navigation, subtle reveal animation, form demo message
- `assets/art/` — put studio-created artwork here

## Color palette

The CSS variables are at the top of `styles.css`. The blue, cyan, pink, and yellow values are sampled directly from `logo.png`. Yellow appears in the supplied logo; the surrounding design uses blue and pink. Headers and footers display the original logo image.

```css
--ink: #07182f;
--blue: #103dd4;
--blue-soft: #00bbff;
--rose: #ff38d4;
--rose-soft: #ff38d4;
--yellow: #fff700;
```

## Replacing an art placeholder

Example for the homepage hero:

```html
<div class="hero-art has-image">
  <img src="assets/art/home-hero.webp" alt="Description of the studio artwork">
</div>
```

Example for a project card:

```html
<div class="project-card-art">
  <img src="assets/art/project-name.webp" alt="Project Name gameplay screenshot">
</div>
```

Recommended formats: AVIF or WebP for images, MP4/WebM for short muted hero reels. Create separate mobile crops for important key art if needed.

## Content pass before launch

Replace all bracketed content with text, names, project facts, location, contact details, and links. Unconfigured external links are displayed as non-clickable placeholders. Connect the contact form to a real backend. Add favicon/OG images and metadata. Test keyboard navigation, image alt text, mobile crops, performance, and reduced-motion behavior.

## Local preview

From this folder:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Header logo and custom lettering

Each header displays `logo.png` as the full symbol, followed by `wordmark.png` as the studio name. Add your text-only image as `wordmark.png` in the project root, alongside `logo.png`. Both images fit their slots without cropping or stretching. Use transparent, tightly cropped assets. Until the wordmark is added, its alternative text identifies the studio as Multiprism.
