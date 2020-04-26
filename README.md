# TAU LaTeX Thesis Template

This is meant to be a minimalistic thesis template to Tampere University (TAU) theses and reports. The current template is made to match the Hervanta campus thesis writing guide as closely as possible.

If you're just getting started or want to know something spesific, I highly recommend you check out the wiki for this project: https://github.com/kulmajaba/tau-thesis-template/wiki

The main document `main.tex` is used by default. `main-min.tex` is a minimalistic document with just the bare essentials (add your own imports as you need them). You can delete the unused main document or keep it around as an example.

I sincerely hope you will find this template useful in completing your thesis project. The document is commented extensively to clarify what everything is doing and give you an idea of how to effectively modify it. Most of the magic happens in the class file, `tauthesis.cls`, which you are more than welcome to take a look at.

I wish you and your project the best of luck! If this template causes you trouble along the way or if you've any suggestions for improving it, please open an issue on GitHub: https://github.com/kulmajaba/tau-thesis-template

## Notice

This template or its associated class file don't come with a warranty. The content is provided as is, without even the implied promise of fitness to the mentioned purpose. You, as the author of the thesis, are responsible for the entire work, including the provided material. No one else is liable to you for any damage inflicted on you or your thesis, were it caused by using this template or not.

## Compiling

Overleaf will compile the template automatically.

If you have an editor that has built-in compiling tools, you can likely work with those. latexmk should work everywhere, and you can always define your own recipe.

Compiling from the command line:

```
pdflatex main.tex
makeindex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

or using latexmk (requires Perl)

```
latexmk
```

## Notes

Please read through the entire template (files under `./tex`) to find all instructions. It is possible that the attached pdf files do not include the latest information.

The GitHub Wiki ans Issues will likely provide more information about specific things that are not written as comments in the tex files.

## Contributing

All contributions are welcome! If you have an issue with the template or notice something is missing (in the wiki for example), please open an issue on GitHub. If you think you can solve it yourself, send in a PR!

## Contributors

Contributions to this project have been made by:

Mika Kuitunen

Ville Koljonen

Jaakko Rinta-Filppula