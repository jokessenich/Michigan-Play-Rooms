# michiganplayrooms.com

Single-page site for Michigan Playrooms — custom indoor play structures, Ann Arbor MI.
A division of Kessenich Carpentry.

No build step, no dependencies. One HTML file plus images.

```
index.html          the whole site — markup, styles and script
img/
  playroom-hero.jpg   hero photo, my basement
  story.jpg           wide shot for the story section
  detail-net.jpg      rope net detail
  detail-nook.jpg     reading nook detail
  concept.jpg         design concept render (labelled as such on the page)
  mark.png            logo mark, transparent
  logo-lockup.png     full logo, transparent
  favicon.png         browser tab / home screen icon
```

## Deploying

Drag the folder into Netlify, Vercel or Cloudflare Pages. Point
michiganplayrooms.com at it. Nothing to configure.

To preview locally:

```
python3 -m http.server 8000
```

then open http://localhost:8000

## Editing

**Build slots.** Search `EDIT THESE TWO LINES` in index.html. Update the season, the
count, and the filled bars as jobs book. Keep it true.

**Prices.** Search `most rooms land between` in the How It Works section.

**Form.** Posts to Formspree at `xjyvegab`. Search `var ENDPOINT` to change it.
Fields are name, city, email, phone.

**Colours.** All in `:root` at the top of the stylesheet.
Ground `--cream`, accent `--glow`, plus six climbing-hold colours `--h1c` to `--h6c`.

**Type.** Archivo Expanded for display, Karla for body, loaded from Google Fonts.
`font-picker.html` in the project history has alternatives if you want to change it.

## Notes

- `concept.jpg` is a design render, not a finished build, and is captioned that way
  on the page. Swap it for a real photo once a job is complete.
- The logo is raster. Get a vector version from the designer before ordering any
  signage, decals or shirts.
- The drawing in the How It Works section is an SVG drawn inline — no image file.
  Edit the geometry constants at the top of the `<svg>` block if the standard
  layout changes.
