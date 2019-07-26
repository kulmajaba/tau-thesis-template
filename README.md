# TAU LaTeX Thesis Template

This is meant to be a minimalistic thesis template to Tampere University (TAU) theses and reports.

Main document class and document: `tauthesis.cls` and `main.tex`. Used by default.

Minimalist class and main document where imports can be removed more easily: `tauthesis-min.cls` and `main-min.tex`. Remember to remove the default document class (and preferably the default main document) If using these.

## Citation

- Numerical and Author-year
- Particles in author names: https://academia.stackexchange.com/questions/15326/how-to-deal-with-particles-in-a-last-name-in-a-reference-list
  - In references.bib: `author = {Abby Muricho Onencan and Bartel {Van de Walle}}`
- "Pieni yksityiskohta on, että suomenkielisen teoksen sivut on ilmoitettu lyhenteellä s. ja englanninkielisen joko lyhenteellä p. (sivumäärä) tai pp. (sisäsivut)."
  - In references.bib: `language = {english}`
- Pagetotal
  - In references.bib: `pagetotal = {300}`

## Notes

- To print all references: `\nocite{*}` before `\printbibliography`

### Biblatex

- Package options:
  - doi: print DOI field, [false, true]
  - isbn: print ISBN field, [false, true]
  - sorting: sort bibliography, multiple options

- Options to research:
  - uniquename
  - maxbibnames
  - sortcites

- adddot: after a shortened word, otherwise addperiod

## Version History
Version 1.0 through 1.3 made by Ville Koljonen

### 1.4
- Continue to fix bibliography styles

### 1.3
- Some updates to appearance
- Removed front matter entries from ToC
- Fixed a problem with default document class options

### 1.2
- Updated the template to conform to new appearance guidelines
- Increased the width of the glossary for it to take less space
- Added compilation instructions to main.tex as well
- Fixed encoding issues relating to listings fix for Scandinavian letters in code comments

### 1.1
- Replaced the glossaries package option xindy to automake. Now the template does not require Perl to be installed
- Added instructions how to compile the thesis using this template into the conclusion text

### 1.0
- First published template
