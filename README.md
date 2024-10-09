# moderncode

This Latex package aims to display code in a beautiful way.

## What does this package do?

This package provides `tcolorbox` environments for block and inline code, as well as `lstlisting` styles. This package loads [`tcolorbox`](https://www.ctan.org/pkg/tcolorbox), [`listings`](https://ctan.org/pkg/listings) and [`xcolor`](https://ctan.org/pkg/xcolor).

## How do I use this package?

First, add the `moderncode.sty` file to your project, and include it via

```tex
\usepackage{moderncode}
```

Now, you can use the environments `moderncode` and `moderncodeout`, as well as the commands `moderncodeinline`, `moderncodeinput` and `moderncodekey`. If you wish to use `lstlisting` instead, you can do that as well. This package also provides a pseudo language style called `pseudo`.

The `moderncode` environment has two optional parameters.
The first argument will be passed to the underlying `listing`, while the second will be passed to the `tcolorbox`.
However, the first argument has another important aspect to note: while it accepts a list of keys, the first key will *always* be passed to the language property.
This is done for ease of use, as usually no further keys are required.

### `moderncode`

![moderncode](https://github.com/Smonman/moderncode/assets/36928284/7d2cde25-9cdb-4c5f-b9b9-d2d851be498f)

### `moderncodeout`

![grafik](https://github.com/Smonman/moderncode/assets/36928284/af6a1d87-7c17-49e4-8fae-df5a15ad48dc)

### `moderncodeinline`

![grafik](https://github.com/Smonman/moderncode/assets/36928284/bb4e1d6c-7cf3-43d6-a054-c0d9db0c30d7)

### `moderncodekey`

![grafik](https://github.com/Smonman/moderncode/assets/36928284/003b1408-d9ac-4be2-8612-795bc54bcefe)

## Changelog

### 0.5.0

- minute spacing adjustments
- add new dedicated argument for the language
- add `escapechar` `!`
- adjust `escapeinside` to be `<*` and `*>` respectively. The old values `(*` and `*)` could lead to errors when displaying C code with function pointers, and some IDEs might complain about improper parenthesis placement.
- the `skins` library from `tcb` is now also loaded
- the styles of `moderncode`, `moderncodeinline` and `moderncodekey` can now be accessed via the keys `/tcb/moderncode`, `tcb/moderncode/inline` and `tcb/moderncode/key/` respectivly.
- remove `breakable` keyword from `moderncode`, `moderncodeout` and `\moderncodeinput` as it could break when used in `tcbraster` or inside of `minipage`. Use `breakable=true` in order to restore old behavior.

### 0.4.1

- add `.chktexrc` file

### 0.4.0

- add `moderncodeinput`

### 0.3.0

- add `mathescape` to standard `lstlisting` style
- change the arguments of the `moderncode` and `moderncodeout` environment to be optional. The first argument controls settings for the internal `listing`. The first entry will always be interpreted as a language. The second optional argument controls settings for the `tcolorbox`

### 0.2.0

- add optional argument for the language for the `moderncodeinline` command
- add local latex indent config file
- fix typos

### 0.1.0

initial version
