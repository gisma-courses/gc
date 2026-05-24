# Course Website

This repository contains the Quarto-based course website.

The site is generated with [Quarto](https://quarto.org/) and published as a static website via GitHub Pages.

## Structure

The main website configuration is handled through:

```text
_quarto.yml
````

Course entries, links, images and descriptions are stored separately in:

```text
_data/courses.yml
```

The homepage reads this YAML file and renders the course sections automatically. To add, remove or edit a course, edit `_data/courses.yml` rather than changing the page template.

## Editing Content

Typical content is stored as Quarto Markdown files:

```text
*.qmd
```

Images and other assets are stored under:

```text
assets/
```

A usual workflow is:

```text
edit .qmd files
→ update _data/courses.yml if course cards change
→ render with Quarto
→ publish generated site
```

## Local Preview

To preview the website locally:

```bash
quarto preview
```

To render the site:

```bash
quarto render
```

## Deployment

The rendered website can be deployed through GitHub Pages. Depending on the repository setup, deployment may use GitHub Actions.


## Credits and History

This course website originally started from the Jekyll implementation of the **Forty** theme by **Andrew Banchich**, based on the original **Forty** theme by HTML5 UP.

```text
Jekyll adaptation:
Andrew Banchich
forty-jekyll-theme
https://github.com/andrewbanchich/forty-jekyll-theme
````

```text
Original theme:
Forty by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license
```

The current version has been substantially reworked and migrated to Quarto. The repository history and contributor list may still reflect the original Jekyll-based origin.
