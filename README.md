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

### `moderncode`

![moderncode](https://github.com/Smonman/moderncode/assets/36928284/7d2cde25-9cdb-4c5f-b9b9-d2d851be498f)

### `moderncodeout`

![grafik](https://github.com/Smonman/moderncode/assets/36928284/af6a1d87-7c17-49e4-8fae-df5a15ad48dc)

### `moderncodeinline`

![grafik](https://github.com/Smonman/moderncode/assets/36928284/bb4e1d6c-7cf3-43d6-a054-c0d9db0c30d7)

### `moderncodekey`

![grafik](https://github.com/Smonman/moderncode/assets/36928284/003b1408-d9ac-4be2-8612-795bc54bcefe)

## Changelog

### 0.1.0

initial version
