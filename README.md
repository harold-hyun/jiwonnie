# 🌸 Bloom & Co. — Flower Business Website

A clean, elegant website for a small floral business. Built with plain HTML & CSS — no frameworks, no build step.

## Getting Started

1. Clone this repo
2. Open `index.html` in your browser
3. Done — no install needed!

## Customizing

### Things to update in `index.html`:
- Replace **"Bloom & Co."** with your actual business name (Ctrl+F → replace all)
- Replace **`@yourusername`** and all Instagram URLs with your real Instagram handle
- Update **[Your City]**, **[Name]**, and the About section text
- Update **prices** in the Arrangements section
- Add your own **photos** (see below)

### Adding photos

There's an `images/` folder (create it) where you can put your photos:

```
flower-site/
  images/
    about.jpg       ← your photo / behind the scenes
    bouquet.jpg     ← classic bouquet
    arrangement.jpg ← vase arrangement
    custom.jpg      ← custom order / any arrangement
```

Then in `index.html`, find the comment `<!-- Replace this div with:` and swap the placeholder divs for real `<img>` tags.

### Changing colors

Open `style.css` and edit the CSS variables at the top:

```css
:root {
  --cream:    #faf6f1;   /* page background */
  --sage:     #8a9e7e;   /* green accent */
  --blush:    #e8c4b0;   /* soft pink */
  --clay:     #c4836a;   /* warm orange-red */
  --ink:      #2b2520;   /* dark text / footer bg */
}
```

## Deploying to GitHub Pages

1. Create a new repo on GitHub (e.g. `bloom-co`)
2. Push this folder to it:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOURUSERNAME/bloom-co.git
   git push -u origin main
   ```
3. Go to **Settings → Pages** in your GitHub repo
4. Set source to **Deploy from a branch → main → / (root)**
5. Your site will be live at `https://YOURUSERNAME.github.io/bloom-co/`

## Contact Form

The form uses `data-netlify="true"` — this only works if you deploy on **Netlify** (also free).

If staying on GitHub Pages, you can use a free form service instead:
- [Formspree](https://formspree.io) — free tier handles 50 submissions/month
- Replace `<form ... data-netlify="true">` with `<form action="https://formspree.io/f/YOUR_ID" method="POST">`

## File Structure

```
flower-site/
  index.html   ← all your content / structure
  style.css    ← all your styles
  images/      ← add your photos here
  README.md    ← this file
```
