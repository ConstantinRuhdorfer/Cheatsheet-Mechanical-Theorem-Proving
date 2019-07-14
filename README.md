# Cheatsheet-Mechanical-Theorem-Proving

This repo holds a cheatsheet containing everything related to the field of mechanical theorem proving that is relevant to my work.
At the moment this reflects ongoning work.

## Quick note on contributing

If you feel like there is a mistake on this cheat sheet or there is room for improvement just do the usual issue/pull request. I appreciate all contributions!

## Useful pre-commit hook

I use this pre-commit hook to automaticly render a pdf from the notebooks markdown since a notebook file is not easily human readable without having jupyter notebook installed.
Also for just reading opening a pdf > running a jupyter notebook server.

```bash
#!/bin/sh
echo "nbconvert converting .ipynb to .pdf ..."
jupyter nbconvert "Cheatsheet Mechanical Theorem Proving.ipynb" --to pdf
git add "Cheatsheet Mechanical Theorem Proving.pdf"
echo "Converted and added to commit."
```
