# Simplistic BibTex Formatter

## Installation

```bash
composer global require leonickl/bibtex-formatter
```

## Usage

```bash
format-bibtex literature.tex [--save|--print|--log|--dump]
```

- `--print` prints the result to the console (**default** option)
- `--save` overrides the original file
- `--log` prints a step-wise info about each token and the current state of the app
- `--dump` dumps the resulting PHP datastructure to the console

**Warning:** The original file will be overwritten by this!

## Features

This formatter only supports simple entries of the form

```bibtex
@type{reference,
    key = {value},
    other = 5,
    ...
}
```

The formatter

- adds trailing commas,
- aligns `=` signs above each other,
- and sets indentation to 4 spaces.
- ...
