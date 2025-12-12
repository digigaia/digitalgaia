# DigitalGaia documentation

## What is it?

This repository contains the information pertaining to the organization of the
DigitalGaia collective.

It is written using the [Sphinx](https://www.sphinx-doc.org/) documentation
system using the [MyST plugin](https://myst-parser.readthedocs.io/), allowing
pages to be written either in the `rst` format or the `markdown` format.


## Build documentation

Start by creating a virtualenv and installing the requirements:

```{sh}
uv sync
```

Build the documentation using

```{sh}
uv run make clean  # optional, never hurts though :)
uv run make html
```

Run a development version that auto-reloads when changes are saved

```{sh}
uv run make clean  # optional, never hurts though :)
uv run make html
uv run python run_livereload.py
```

## TODO / FIXME

- check other themes for doc: <https://github.com/lepture/shibuya>, others...

- check other fonts for styling the documentation
  https://beautifulwebtype.com/

  https://fonts.google.com/specimen/Exo+2

  normal: Inter, Roboto Slab, Noto, Merriweather, Lato, Caslon, Open Sans, Cantarell, Menlo, Titillium Web, Saira Semi Condensed, Cronos Pro (check https://v4.chriskrycho.com/2019/cronos-follow-up.html though)

  heading: CooperBT, Averia

  maybe use <https://modernfontstacks.com/>

- remove unused fonts from `custom.css` and `_static/fonts` folder
