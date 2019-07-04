# @ac-ui/design-system

A SCSS design system based on Bootstrap, to provide styling and theming to all Avenue Code products

# TODO
1. Add editor config files
2. Add linting config files

# Installation
1. Install as a npm dependency `npm i git+ssh://git@gitlab.com:acbr/internal/ac-ui/design-system.git`
2. Use within your SCSS 
    - Want settings, mixins, extends, with no classes? 
        - `@import "~@ac-ui/design-system/src/base";`
    - Want access to Bootstrap's grid classes?
        - No need to import the `required` partial!
        - `@import "~@ac-ui/design-system/src/bridge/grid";`
    - Want to load everything? Please reconsider.
        - `@import "~@ac-ui/design-system/src";`

# Overview
- `src/index.scss` -> Entry file into all utility files/classes
- `src/_variables.scss` -> Baseline theme variables. Product implementation can override.
- `src/bridge/${FILE_NAME}` -> Act as a bridge file to Bootstrap, add pertinent styles
    - Each bridge file loads AC-UI Variables, and has access to all Mixins/Functions/Variables
