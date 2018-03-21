# Pandoc Markdown

Syntax highlighting for [Pandoc's Markdown](https://pandoc.org/MANUAL.html#pandocs-markdown).

Currently supported:
* Citations
* Footnotes
* Inline math: `$...$`
* Display math: `$$\n...\n...\n$$`

Not yet supported, in rough order of priority:
1. Inline attribute spans: `{#identifier .class .class key=value key=value}`
2. Fenced divs
3. Bracketed spans
4. Subscripts and superscripts
5. Fancy lists
6. Line blocks
7. Definition lists
8. Example lists
9. Tables
10. Strikeouts

# Credits

Based on Microsoft's [VS Code markdown extension's Textmate grammar](https://github.com/Microsoft/vscode-markdown-tm-grammar) and Lukas Eipert's [language-pfm](https://github.com/leipert/language-pfm).

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
