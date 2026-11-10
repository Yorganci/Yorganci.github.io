# yorganci.github.io

Personal portfolio of **Bunyan Yorganci**, a Computer Systems Engineering student at Carleton University.

**Live site:** https://yorganci.github.io

The site covers embedded and systems projects (the SYSC 4805 autonomous snowplow robot, an OS/interrupt simulator, Linux IPC, Raspberry Pi hardware, software validation), along with my background, coursework and resume.

## Structure

```
index.html        Home: intro, featured projects, skills, experience
projects.html     All project case studies, with category filters
about.html        Background, education, experience, coursework
assets/
  css/portfolio.css   All styling (single stylesheet, no framework)
  images/             Project diagrams (SVG) and photos
  docs/               Public resume PDF
```

It's a plain static site: hand-written HTML and CSS, with a few lines of vanilla JavaScript for the project filters. There's no build step and nothing to install.

## Running locally

Open `index.html` in a browser, or serve the folder so links behave as they do on GitHub Pages:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

GitHub Pages publishes the `main` branch automatically. Changes are live a minute or two after pushing.

## Updating

- **Add a project:** copy an existing `<article class="case">` block in `projects.html`, give it a unique `id` and a `data-cat` (`systems`, `embedded`, `verification`, `signals` or `personal`), and link to it from `index.html` as `projects.html#<id>`.
- **Update the resume:** replace `assets/docs/Bunyan_Yorganci_Resume_Public.pdf` and keep the same file name. The public version leaves out my phone number.
- **Change colours or fonts:** edit the variables at the top of `assets/css/portfolio.css`.

## Credits

Design and development by Bunyan Yorganci. Typefaces: [IBM Plex](https://github.com/IBM/plex) (SIL Open Font License), served from Google Fonts.

Found a problem? [Open an issue](https://github.com/Yorganci/yorganci.github.io/issues).

© 2026 Bunyan Yorganci. Site content is not licensed for reuse.
