# TOON Syntax Highlighting for Sublime Text

Syntax highlighting package for [TOON (Token-Oriented Object Notation)](https://github.com/toon-format/toon) format in Sublime Text.

## Features

- **Complete syntax highlighting** for TOON format files (`.toon`)
- **Semantic coloring** for:
  - Array declarations with length indicators `[N]`
  - Tabular field definitions `{field1,field2,field3}`
  - Key-value pairs and nested objects
  - Delimiter detection (comma, tab, pipe)
  - Dotted path key folding `data.metadata.items`
  - List items with `- ` markers
  - Strings (quoted and unquoted)
  - Numbers, booleans, and null values
  - Escape sequences in strings
- **Multiple delimiter support**: comma (`,`), tab (`\t`), and pipe (`|`)
- **Custom color scheme** optimized for TOON readability

## Installation

1. Press `Ctrl+Shift+P` to open the Command Palette
2. Type **Add Package** and select it
3. Select **Install Package**
4. Search for and select **toon**

## Color Scheme Customization

The package includes a default color scheme. To customize colors:

1. Open `TOON.sublime-color-scheme`
2. Modify the `variables` section to change colors:

```json
"variables": {
  "blue": "#4FC3F7",      // Keys and array names
  "green": "#81C784",     // Strings
  "orange": "#FFB74D",    // Numbers and field definitions
  "red": "#E57373",       // Invalid/errors
  "purple": "#BA68C8",    // Booleans, null, array lengths
  "cyan": "#4DD0E1",      // Dotted paths, escapes
  "yellow": "#FFF176",    // List markers
  "grey": "#B0BEC5"       // Separators, comments
}
```

## Syntax Scopes

The following scopes are defined for theme customization:

- `variable.other.array-name.toon` - Array names
- `variable.other.key.toon` - Object keys
- `variable.other.dotted-path.toon` - Dotted key paths
- `constant.numeric.array-length.toon` - Array length numbers `[N]`
- `meta.array-fields.toon` - Field definitions `{field1,field2}`
- `keyword.operator.delimiter.toon` - Delimiter indicators
- `string.quoted.double.toon` - Quoted strings
- `string.unquoted.toon` - Unquoted strings
- `constant.numeric.toon` - Number literals
- `constant.language.boolean.toon` - `true`/`false`
- `constant.language.null.toon` - `null`
- `punctuation.definition.list-item.toon` - List markers `- `
- `punctuation.separator.*.toon` - Value separators
- `constant.character.escape.toon` - Escape sequences
- `comment.line.toon` - Comments (unofficial extension)

## TOON Format Resources

- **Official Repository**: https://github.com/toon-format/toon
- **Specification**: https://github.com/toon-format/spec
- **Documentation**: https://toonformat.dev
- **NPM Package**: [@toon-format/toon](https://www.npmjs.com/package/@toon-format/toon)

## License

MIT License - Feel free to use and modify

## Credits

Based on the [TOON Format Specification](https://github.com/toon-format/spec) (v2.0) by the TOON Format community.
