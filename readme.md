# Game Design Document Template

This is intended to be a template for game design documents written in LaTeX. On top of providing additional utilities for writing GDDs, sections are provided as an example and may be modified or reordered as needed.

Notable features:
- supports various inline images for things like controller buttons or dice icons. Include `\input{latex/demos/inline_graphics}` for a full list.
- automatically adds a changelog based on git history, if available. If this isn't in a git repo then it'll still work, there just won't be a changelog.

## How to Compile

This uses the LaTeX package [minted](https://github.com/gpoore/minted) and as such requires the python module `Pygments` (installable with `pip install Pygments`), and that compiling of the document requires the `--shell-escape` flag.

It also uses `biber` rather than `bibtex` for git logs.
