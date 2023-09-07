# IEL project, version 2022/01

This document describes the IEL project.

## Usage
### Overleaf
To import into Overleaf, remove the `packages` directory and the `latexmkrc` file from the downloaded template and repack the modified template as a zip. After that, just click on the New project button in the project overview --> Upload --> drag the zip. The template will be ready to use. Rename the newly created project with your login.

### Locally
Just unzip the zip archive to any folder. It can also be translated from the command line. All you need for this template is:
```
pdflatex 00-project.tex xonufr00.pdf

pdflatex 00-project.tex xonufr00.pdf
```
If you want to use the circuitikz package with parameters in the template, use:

`latexmk -pdf 00-project.tex`

the `latexmk` command compiles the project with the circuitikz package that comes with the template.

# Project structure
This section of the README file briefly introduces the structure of the project.

* fig
  Directory with images. Contains the FIT BUT logo in the Czech and English versions and circuits for individual examples
* packages
  Directory with packages that may not be part of the LaTeX installation. The latest version of the circuitikz package is currently attached. Additional packages can be added as needed.
* root directory
  The root directory contains the following files that students modify:
  * 00-project.tex
     Basic template file. It contains basic settings, a header and documents with examples are inserted into it. Apart from the header and possible language settings, there is no need to change this file.
  * 01-pr1.tex -- 05-pr5.tex
     Files that contain individual examples. The parameter of the firstEntry, secondEntry commands determines which entry is placed in the entry table and which group is added to the response table.
  * 06-tab.tex
     The file that contains the response table. Groups should be added automatically, you only add results and units.
* Additional files in the root directory that do not need to be modified:
  * wick.cls
     Definition of document style.
  * latexmkrc
     Settings for the latexmk utility (location of packages, packages subfolder).
  * README.md
     This document.

# Other sources of information
I highly recommend the web book https://en.wikibooks.org/wiki/LaTeX if you are new to LaTeX. If you're having trouble, google it.

# Author
Ivan Onufriienko(xonufr00@fit.vut.cz) is solely responsible for the project, please direct all questions to him.
