# latex-template
The LaTeX template that I use for my university assignments.

[Example PDF here](https://users.dcc.uchile.cl/~ereyes/web/viewer.html?file=template.pdf)

## Features

1. Title page with logo of your choice.
2. Support for mathematical environments with correct enumeration.
3. Support for source code in multiple languages thanks to *[minted](https://www.overleaf.com/learn/latex/Code_Highlighting_with_minted)*.
4. Automated support for bibliographies in APA format.

## Requirements

### Working online

We can work with this template directly on [Overleaf](https://www.overleaf.com/). To do this, we must upload it as a project and remove the parameter `[outputdir=build]` from `[\usepackage[outputdir=build]{minted}]` in `[/lib/packages.tex]`

### Working locally

1. Install [TexLive](https://www.tug.org/texlive/)
2. Install [Python](https://www.python.org/downloads/) and Pygments (`pip install Pygments`) if we are going to use the *minted* package.
3. (Optional) Install the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension in [Visual Studio Code](https://code.visualstudio.com/download).
4. Compile with the *pdftex* recipe for a simple document. Compile *pdftex* twice to correctly enumerate references and compile together with *bibtex* to obtain a correctly formatted bibliography (The buttons and macros for *LaTeX Workshop* are already included in the Workspace folder `[.vscode]`).
5. (Optional) If you want to use *synctex* with external *PDF* viewers, I recommend [this guide](https://github.com/James-Yu/LaTeX-Workshop/wiki/View#using-synctex-with-an-external-viewer).

## License

This code is distributed under the MIT license. For more info, read the [LICENSE](/LICENSE) file distributed with the source code.
