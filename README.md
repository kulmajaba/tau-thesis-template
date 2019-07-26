# TAU LaTeX Thesis Template

This is meant to be a minimalistic thesis template to Tampere University (TAU) theses and reports. The current template is made to match the Hervanta campus thesis writing guide as closely as possible.

Main document class and document: `tauthesis.cls` and `main.tex`. Used by default. Minimalist document with just the bare essentials (add your own imports as you need them):`main-min.tex`. You can delete the unused main document or keep it around as an example.

Congratulations, you've made an excellent choice of writing your Tampere University thesis using the LaTeX system. This document attempts to be as complete a template as possible to let you focus on the most important part: the writing itself. Thus the details regarding the visual appearance and even structure have already been worked out for you!

I sincerely hope you will find this template useful in completing your thesis project. I've tried to add comments (followed by the % sign) to clarify the structure and purpose of some of the commands. Most of the magic happens in the file tauthesis.cls, which you are more than welcome to take a look at. Just refrain from editing it in the most crucial versions of the thesis!

I wish you and your thesis project the best of luck! If this template causes you trouble along the way or if you've any suggestions for improving it, please open an issue on GitHub: https://github.com/kulmajaba/tau-thesis-template

## Notice

This template or its associated class file don't come with a warranty. The content is provided as is, without even the implied promise of fitness to the mentioned purpose. You, as the author of the thesis, are responsible for the entire work, including the provided material. No one else is liable to you for any damage inflicted on you or your thesis, were it caused by using this template or not.

## Contributing

All contributions are welcome! If you have an issue with the template or notice something is missing (in the wiki for example), please open an issue on GitHub. If you think you can solve it yourself, send in a PR!

## Notes

Please read through the entire template (files under ./tex) to find all instructions. It is possible that the attached pdf files do not include the latest information.

### Compiling

Overleaf: just click Recompile.
Terminal:
 1. `pdflatex main.tex`
 2. `makeindex main.tex`
 3. `biber main.tex`
 4. `pdflatex main.tex`
 5. `pdflatex main.tex`
Similar sequence of commands is also required
in LaTeX specific editors.

### Citation

Supported styles are numerical and author-year

- Particles in author names: https://academia.stackexchange.com/questions/15326/how-to-deal-with-particles-in-a-last-name-in-a-reference-list
  - In references.bib: `author = {Abby Muricho Onencan and Bartel {Van de Walle}}`
- "Pieni yksityiskohta on, että suomenkielisen teoksen sivut on ilmoitettu lyhenteellä s. ja englanninkielisen joko lyhenteellä p. (sivumäärä) tai pp. (sisäsivut)."
  - In references.bib: `language = {english}`
- Pagetotal
  - In references.bib: `pagetotal = {300}`
- To print all references: `\nocite{*}` before `\printbibliography`

### Biblatex

- adddot: after a shortened word, otherwise addperiod

## Version History

### 1.5
- Move all of the extra packages to main.tex and strip down tauthesis.cls to essentials, add a truly minimalistic main-min.tex

### 1.4
- Continue to fix bibliography styles

### 1.3 (authored by Ville Koljonen)
- Some updates to appearance
- Removed front matter entries from ToC
- Fixed a problem with default document class options

### 1.2 (authored by Ville Koljonen)
- Updated the template to conform to new appearance guidelines
- Increased the width of the glossary for it to take less space
- Added compilation instructions to main.tex as well
- Fixed encoding issues relating to listings fix for Scandinavian letters in code comments

### 1.1 (authored by Ville Koljonen)
- Replaced the glossaries package option xindy to automake. Now the template does not require Perl to be installed
- Added instructions how to compile the thesis using this template into the conclusion text

### 1.0 (authored by Ville Koljonen)
- First published template
