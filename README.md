# TAU LaTeX Thesis Template

This is meant to be a minimalistic thesis template to Tampere University (TAU) theses and reports.


## TODO

- tauthesis.cls: @-letters have been removed from conditional variables, do they need to be returned?
- tauthesis.cls: build fails if the class is given one of the default options in main.tex

### Citation styles: general
- Numerical and Author-year
- https://academia.stackexchange.com/questions/15326/how-to-deal-with-particles-in-a-last-name-in-a-reference-list
  - In references.bib: `author = {Abby Muricho Onencan and Bartel {Van de Walle}}`
- URL style after books etc.
- "Pieni yksityiskohta on, että
suomenkielisen teoksen sivut on ilmoitettu lyhenteellä s. ja englanninkielisen joko
lyhenteellä p. (sivumäärä) tai pp. (sisäsivut). Kokonaissivumäärän ilmoittaminen ei ole
pakollista, mutta se antaa lukijalle pientä vinkkiä lähteen laajuudesta."
  - In references.bib: 

### Citation styles: numerical

### Citation styles: author-year


## Notes

- adddot: after a shortened word, otherwise addperiod

## Version History
Version 1.0 through 1.2 made by Ville Koljonen

### Version 1.0
- First published template.

### Version 1.1
- Replaced the glossaries package option xindy to automake. Now the template does not require Perl to be installed.
- Added instructions how to compile the thesis using this template into the conclusion text.

### Version 1.2
- Updated the template to conform to new appearance guidelines.
- Increased the width of the glossary for it to take less space.
- Added compilation instructions to main.tex as well.
- Fixed encoding issues relating to listings fix for Scandinavian letters in code comments.