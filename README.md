# Pandoc Flavored Markdown

Syntax highlighting for [Pandoc's Markdown](https://pandoc.org/MANUAL.html#pandocs-markdown).

Supported:
* Citations
* Footnotes

Not yet supported:
* Inline attribute spans (`{#identifier .class .class key=value key=value}`)
* Line blocks
* Fancy lists
* Definition lists
* Example lists
* Tables
* Strikeouts
* Subscripts and superscripts
* Math mode
* Fenced divs
* Bracketed spans

# Credits

Based on Microsoft's [VS Code markdown extension's Textmate grammar](https://github.com/Microsoft/vscode-markdown-tm-grammar).

# Known Issues

* Inline footnotes spanning multiple lines only get highlighted up to the first line break

# Contributing

The main grammar is stored in `syntaxes/markdown.tmLanguage.json`. This file is generated from `markdown.tmLanguage.base.yaml`:

## Building

To generate the main grammar:

```bash
$ npm install
$ npm run build 
```

## Testing

To run the grammar tests:

```bash
$ npm run test
```
