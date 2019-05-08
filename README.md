# TAU LaTeX Thesis Template

This is meant to be a minimalistic thesis template to Tampere University (TAU) theses and reports. The current template is made to match the Hervanta campus thesis writing guide as closely as possible.

Main document class and document: `tauthesis.cls` and `main.tex`. Used by default.

Minimalist class and main document where imports can be removed more easily: `tauthesis-min.cls` and `main-min.tex`. Remember to remove the class and the main document you are not using, and rename the used class and document to `tauthesis.cls` and `main.tex`

## Citation

Supported styles are numerical and author-year

### Notes

- Particles in author names: https://academia.stackexchange.com/questions/15326/how-to-deal-with-particles-in-a-last-name-in-a-reference-list
  - In references.bib: `author = {Abby Muricho Onencan and Bartel {Van de Walle}}`
- "Pieni yksityiskohta on, että suomenkielisen teoksen sivut on ilmoitettu lyhenteellä s. ja englanninkielisen joko lyhenteellä p. (sivumäärä) tai pp. (sisäsivut)."
  - In references.bib: `language = {english}`
- Pagetotal
  - In references.bib: `pagetotal = {300}`

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

## Development

### Roadmap

- Move Todos and new issues to issue tracker
- Contribution guide
- Documentation in wiki
  - Basic usage
  - Adding graphics
  - Adding formulas
  - Listings
  - `biblatex` usage
  - Customization
  - 
- Strip tauthesis-min down to bare essentials
- Introduce an alternative to `listings`, possibly with `minted`
- Figure out the best way of maintaining tauthesis/main and tauthesis-min/main-min
  - Branches?
  - Forks?
  - Common code base with customization (is this possible with LaTeX classes?)

### Notes

- To print all references: `\nocite{*}` before `\printbibliography`

### Biblatex

- Package options:
  - doi: print DOI field, [false, true], currently false
  - isbn: print ISBN field, [false, true], currently false
  - sorting: sort bibliography, multiple options, currently `nyt` (name-year-title) for author year and `none` for numerical

- Options to research:
  - uniquename
  - maxbibnames
  - sortcites

- adddot: after a shortened word, otherwise addperiod

### TODO

- Leaving any of the fields empty in main.tex (e.g. \\title) will cause an error during compilation. Writing `~` into the field will fix this and the field remains empty
- tauthesis: biblatex: URL will be printed always if available, for all bibtex types. Should this behavior be changed?
- tauthesis: biblatex: DOIs are never printed, should this behavior be changed?
- tauthesis: biblatex: series for thesis and thesis aliases will be printed, is the current format correct?
- tauthesis: biblatex: standard, manual, unpublished formatting
