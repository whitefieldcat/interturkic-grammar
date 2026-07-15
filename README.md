# Interturkic Grammar

## Compilation

Esure that the following dependencies are installed and operational:
- **Compiler:** LuaTeX with support for the HarfBuzz engine.
- **Packages:**
  - [bookmark](https://ctan.org/pkg/bookmark)
  - [booktabs](https://ctan.org/pkg/booktabs)
  - [expex](https://ctan.org/pkg/expex)
  - [extdash](https://ctan.org/pkg/extdash)
  - [fontspec](https://ctan.org/pkg/fontspec)
  - [hyperref](https://ctan.org/pkg/hyperref)
  - [leipzig](https://ctan.org/pkg/leipzig)
  - [longtable](https://ctan.org/pkg/longtable)
  - [luabidi](https://ctan.org/pkg/luabidi)
  - [memoir](https://ctan.org/pkg/memoir)
  - [microtype](https://ctan.org/pkg/microtype)
  - [multirow](https://ctan.org/pkg/multirow)
  - [varioref](https://ctan.org/pkg/varioref)
- **Fonts:**
  - [Noto Naskh Arabic](https://fonts.google.com/noto/specimen/Noto+Naskh+Arabic)
  - [Noto Sans Math](https://fonts.google.com/noto/specimen/Noto+Sans+Math)
  - [Noto Serif](https://fonts.google.com/noto/specimen/Noto+Serif)

In order to compile the document itself, run these commands in order from the
project root:
```
lualatex --draftmode grammar
makeglossaries grammar
lualatex --draftmode grammar
lualatex grammar
```
If successful, `grammar.pdf` should be generated in the same directory.