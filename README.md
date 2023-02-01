# latex-template
La plantilla de LaTeX que uso para mis tareas en la universidad

[Ejemplo en PDF aquí](https://users.dcc.uchile.cl/~ereyes/web/viewer.html?file=template.pdf)

## Características / Features

1. Portada / Title page con logo de la Universidad y departamento a elección.
2. Soporte para herramientas matemáticas con correcta enumeración.
3. Soporte para código fuente de varios lenguajes gracias a [minted](https://www.overleaf.com/learn/latex/Code_Highlighting_with_minted).
4. Soporte para bibliografía en formato APA automatizado.

## Prerrequisitos

### Trabajar de manera en línea

Podemos trabajar con esta plantilla directamente en [Overleaf](https://www.overleaf.com/). Para ello debemos subirla como proyecto y remover el parámetro `[outputdir=build]` de `[\usepackage[outputdir=build]{minted}]` en `[/lib/code.tex]`

### Trabajar de manera local

1. Instalar [TexLive](https://www.tug.org/texlive/)
2. Instalar Python y Pygments (`pip install Pygments`) si vamos a usar el paquete *minted*.
2. (Opcional) Instalar la extensión [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) en Visual Studio
3. Compilar con la receta de *pdftex* para un documento simple. Compilar dos veces *pdftex* para enumerar correctamente referencias y compilar junto a *bibtex* para obtener una bibliografía correctamente (Los botones y macros para *LaTeX Workshop* vienen ya hechos en la carpeta de Workpace `[.vscode]`)
4. (Opcional) Si se desea utilizar *synctex* con visualizadores externos de *PDF* recomiendo [Esta guía](https://github.com/James-Yu/LaTeX-Workshop/wiki/View#using-synctex-with-an-external-viewer)

## License

This code is distributed under the MIT license. For more info, read the
[LICENSE](/LICENSE) file distributed with the source code.
