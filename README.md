# TAU LaTeX Thesis Template

This is meant to be a minimalistic thesis template to Tampere University (TAU) theses and reports.


## TODO

- Leaving any of the fields empty in main.tex (e.g. \\title) will cause an error durring compilation. Writing `~` into the field will fix this and the field remains empty
- tauthesis: biblatex: URL will be printed always if available, for all bibtex types. Should this behavior be changed?
- tauthesis: biblatex: DOIs are never printed, should this behavior be changed?

### Citation styles: general
- Numerical and Author-year
- https://academia.stackexchange.com/questions/15326/how-to-deal-with-particles-in-a-last-name-in-a-reference-list
  - In references.bib: `author = {Abby Muricho Onencan and Bartel {Van de Walle}}`
- URL style after books etc.
- "Pieni yksityiskohta on, että suomenkielisen teoksen sivut on ilmoitettu lyhenteellä s. ja englanninkielisen joko lyhenteellä p. (sivumäärä) tai pp. (sisäsivut)."
  - In references.bib: `language = {english}`
- Pagetotal
  - In references.bib: `pagetotal = {300}`
- standard, manual, unpublished formatting
- URL formatting: book, manual, standard, unpublished

### Citation styles: numerical

### Citation styles: author-year


## Notes

- adddot: after a shortened word, otherwise addperiod

### Biblatex

- Package options:
  - doi: print DOI field, [false, true]
  - isbn: print ISBN field, [false, true]
  - sorting: sort bibliography, multiple options

- Options to research:
  - uniquename
  - maxbibnames
  - sortcites

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