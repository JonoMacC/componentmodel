# Component Model

Language configuration for syntax highlighting on component model specifications. Component models are plain text files that follow a prescribed structured as detailed on [Spire Wiki](https://wiki.spiretrading.com/index.php/Model). This extension enables VS Code to apply syntax highlighting from your chosen theme to model files to emphasize salient information.

## Features

Provides highlighting for:

- Fields: Definitions, Data, State and Signals
- Signals: FocusIn, Delete, MouseMove
- Parameters: current, background_color
- Numbers: 1, 100, 0.5
- Color Hex Codes: #FF, #FFF, #FFFFFF
- Pixel Values: 10px, 2px, 1000px
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

### 0.1.0

Initial release of Component Model.

### 0.1.1

Fix highlighting on enums to exclude colon.

### 0.2.0

Fix highlighting on enums to identify them inside of text.
Add highlighting for regexes.
