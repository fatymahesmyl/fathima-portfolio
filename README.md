# Fathima M — Portfolio Website

A 5-page HTML5 + CSS portfolio: Home, About Me, Achievements, Gallery, Contact Me.

## Files
- `index.html` — Home
- `about.html` — About Me
- `achievements.html` — Achievements
- `gallery.html` — Gallery
- `contact.html` — Contact Me
- `style.css` — shared styling for all pages

## How to publish on GitHub Pages
1. Create a new GitHub repository (e.g. `fathima-portfolio`).
2. Upload all the files above into the **root** of that repository (not inside a subfolder).
3. Go to **Settings → Pages** in the repository.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/root`, then **Save**.
5. Wait about 1 minute, refresh the page — GitHub shows your live URL, usually:
   `https://<your-username>.github.io/fathima-portfolio/`

## Add your own photos (Gallery page)
The gallery currently has placeholder tiles. To use real photos:
1. Add an `assets/` folder to the repo and upload your images there (e.g. `assets/photo-01.jpg`).
2. In `gallery.html`, replace a placeholder tile like:
   ```html
   <div class="gallery-item"><span>photo-01.jpg<br>Campus / College</span></div>
   ```
   with:
   ```html
   <div class="gallery-item"><img src="assets/photo-01.jpg" alt="Describe the photo"></div>
   ```
3. Repeat for each photo.

## Make the contact form actually send email (optional)
The form on `contact.html` is static. To make it work without a backend:
1. Create a free account at formspree.io and create a new form — you'll get a URL like
   `https://formspree.io/f/xxxxabcd`.
2. In `contact.html`, change `<form action="#" method="POST">` to
   `<form action="https://formspree.io/f/xxxxabcd" method="POST">`.
