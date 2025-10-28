# Simplistic BibTex Formatter

## Installation

```bash
composer global require leonickl/bibtex-formatter
```

## Usage

```bash
format-bibtex literature.tex
```

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
