# moderncode

This Latex package aims to display code in a beautiful way.

## What does this package do?

This package provides `tcolorbox` environments for block and inline code, aswell as `lstlisting` styles. This package loads [`tcolorbox`](https://www.ctan.org/pkg/tcolorbox) and [`listings`](https://ctan.org/pkg/listings).

## How do I use this package?

First, add the `moderncode.sty` file to your project, and include it via
```tex
\usepackage{moderncode}
```

Now, you can use the environments `moderncode` and `moderncodeout`, aswell as the commands `moderncodeinline` and `moderncodekey`. If you wish to use lstlistings instead, you can do that aswell. This package also provides a pseudo language style called `pseudo`.

## Changelog

### 0.1.0

initial version
