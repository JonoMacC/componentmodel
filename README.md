# Component Model

Language configuration for syntax highlighting on component model specifications. Component models are plain text files that follow a prescribed structured as detailed on [Spire Wiki](https://wiki.spiretrading.com/index.php/Model). This extension enables VS Code to apply syntax highlighting from your chosen theme to model files to emphasize salient information.

## Features

Provides highlighting for:

- Fields: Definitions, Data, State and Signals
- Signals: FocusIn, Delete, MouseMove
- Parameters: current, background_color, x0
- Numbers: 1, 100, 0.5
- Color Hex Codes: #FF, #FFF, #FFFFFF, 0xFFFFFF
- Unit Values: 10px, 2ch, 5em, 100%, 500ms
- Regex: /^[a-zA-Z0-9]$/
- Enums: NONE, SINGLE, DROP_ALLOWED

## Requirements

To build the extension, you will need to install the dependencies.

```bash
npm install
```

Then run `vsce package` to build it.

```bash
npx vsce package
```

You should see `componentmodel-0.2.0.vsix` saved to the directory. To install, run the command `Extensions: Install from VSIX...` from the VS Code Command Palette and select the package file.

## Extension Settings

To use, set the language in VS Code to "Component Model" for the file you are viewing.

## Release Notes

| Version | Description                                                                                                                                                  |
| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 0.3.3   | Fix minus sign highlights for numbers.                                                                                                                       |
| 0.3.2   | Fix highlights for parameters with no description.                                                                                                           |
| 0.3.1   | Make boolean highlights case-insensitive. Fix single word lines ending in colon being highlighted as parameter.                                              |
| 0.3.0   | Add constant highlights for `h`, `m`, `s`, `ms`. Add highlight support for 0x hex color values. Add highlight support for parameter names containing digits. |
| 0.2.4   | Fix highlighting on enums to highlight wherever they occur. Add constant highlights for `ch`, `em`, and `%`. Add highlights for Booleans.                    |
| 0.2.3   | Add icon.                                                                                                                                                    |
| 0.2.2   | Fix highlighting on enums to exclude single-letters. `A` is no longer highlighted as a constant.                                                             |
| 0.2.1   | Add installation instructions to README.                                                                                                                     |
| 0.2.0   | Fix highlighting on enums to identify them inside of text. Add highlighting for regexes.                                                                     |
| 0.1.1   | Fix highlighting on enums to exclude colon.                                                                                                                  |
| 0.1.0   | Initial release of Component Model.                                                                                                                          |
