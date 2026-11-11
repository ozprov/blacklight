# BLACKLIGHT

Pre-production teaser site for the feature film BLACKLIGHT, a crime drama set in Andamooka, South Australia.

Plain static HTML, CSS and JavaScript. No framework, no build step.

## Run it locally

    python3 -m http.server 8000

Then open http://localhost:8000. Opening `index.html` straight from disk also works, apart from fonts, which load from Google Fonts.

## Layout

- `index.html`: the whole page, with the logo and tagline as inline SVG
- `assets/`: images and the 1950s concept footage used by the page
- `source/`: the supplied logo and tagline SVGs and the original cast photo
- `favicon.svg`

## Adding the trailer

Put the video in `assets/` and set `TRAILER_SRC` near the top of the script in `index.html`, for example `var TRAILER_SRC = "assets/trailer.mp4";`. Until it is set, the play button tells visitors the teaser is still in the edit.

## Expression of interest

The form builds a pre-filled email to info@australianprovenanceproject.com.au. It opens the visitor's email app and sends nothing itself.

## Notes

- Images and footage are concept material from pre-production.
- The synopsis stops before the final act on purpose.
- `.nojekyll` is included in case the site is later served from GitHub Pages.
- No licence file is included.
