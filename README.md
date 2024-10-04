# componentmodel README

Language configuration for syntax highlighting on component model specifications.
Component models are plain text files that follow a prescribed structured as
detailed on https://wiki.spiretrading.com/index.php/Model. This extension enables
VS Code to apply syntax highlighting from your chosen theme to model files to
emphasize salient information.

## Features

Provides highlighting for:

- Entities: top-level fields ('Definitions', 'Data', 'State' and 'Signals')
- Signals: signal names ('FocusIn', 'Delete', 'MouseMove')
- Parameters: component parameters ('current', 'background_color')
- Numbers
- Colors: hex code values (#FF, #FFF, #FFFFFF)
- Pixel values: (10px, 2px, 1000px)
- Defined Enums: preset values (NONE, SINGLE, DROP_ALLOWED)

## Requirements

None.

## Extension Settings

To use, set the language in VS Code to "Component Model" for the file you are
viewing.

## Release Notes

### 1.0.0

Initial release of Component Model.
