# Typst Extension for Zed

## Usage
To register the LSP and enable certain features such as compile on save, add the
following your `settings.json` (or `.zed/settings.json` in the project root for
project-specific config),

```json
"lsp": {
  "tinymist": {
    "initialization_options": {
      "exportPdf": "onSave",
      "outputPath": "$root/$name"
    }
  }
}
```

This will compile a PDF for the `main.typ` file in the project root.

To see all available options refer to [the tinymist documentation](https://github.com/Myriad-Dreamin/tinymist/blob/main/editors/neovim/Configuration.md)

## Components
- Tree Sitter: [tree-sitter-typst](https://github.com/uben0/tree-sitter-typst/)
- Language Server: [tinymist](https://github.com/Myriad-Dreamin/tinymist/)
