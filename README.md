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

## Credits

The visual design is based on the **Forty** theme by [HTML5 UP](https://html5up.net/), adapted for this Quarto-based course website.

Original theme credit:

```text
Forty by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license
```

Theme resources:

```text
Icons: Font Awesome
Original demo image source: Unsplash
Original HTML/CSS/JS base: HTML5 UP Forty
```

Repository icon credit:

The Jekyll logo icon, where still present in inherited assets, is licensed under a Creative Commons Attribution 4.0 International License.
