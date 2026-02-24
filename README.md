# OSIRIS SCSS

SCSS source files for the OSIRIS Research Information System.

This repository contains the styling source code used to generate the compiled CSS that is shipped with the main OSIRIS application.

The compiled CSS files are included in the main OSIRIS repository.  
This repository is only required if you want to develop or modify the styling.


## Requirements

- Dart Sass (recommended)
  https://sass-lang.com/


## Build

From the project root:

```bash
sass main.scss ../osiris/css/main.css --style=compressed
```

Adjust the output path according to your local OSIRIS installation.

For development (with auto-rebuild):

```bash
sass --watch main.scss:../osiris/css/main.css
```


## Workflow
1. Modify SCSS files.
2. Compile CSS.
3. Commit changes:
   - SCSS changes → this repository
   - Generated CSS → main OSIRIS repository


## Versioning Strategy
- SCSS is versioned independently.
- The OSIRIS main repository references a specific SCSS version (via submodule).
- Compiled CSS is committed to the main repository for deployment stability.


## Credits

This styling system incorporates and adapts elements from:
- Halfmoon CSS
- Bootstrap

Both licensed under MIT.

See source headers for detailed license information.
