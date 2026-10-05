# Blowfish site

Website built with [Hugo](https://gohugo.io/) and the [Blowfish](https://blowfish.page/) theme. It covers the docs, sample articles, recipes and a showcase of templates.

## Requirements

- Hugo extended, v0.163 or later
- Git

## Getting started

The theme is installed as a Git submodule in `themes/blowfish`. After cloning, fetch it with:

```sh
git submodule update --init --recursive
```

Run the local development server:

```sh
hugo server
```

Then open http://localhost:1313/.

Build the site for production:

```sh
hugo --gc --minify
```

The output is written to `public/`.

## Project layout

- `config/_default/` — site, language, menu, markup and theme settings
- `content/` — pages and articles (docs, samples, guides, examples, authors, tags)
- `data/authors/` — author profiles used for multi-author articles
- `assets/` — images and scripts processed by Hugo
- `layouts/` — overrides of the theme's templates and a few custom shortcodes
- `themes/blowfish/` — the Blowfish theme (Git submodule, do not edit)

## Updating the theme

```sh
cd themes/blowfish
git fetch --tags
git checkout <new-version-tag>
cd ../..
```
