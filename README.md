# @ac-ui/design-system

A SCSS design system based on Bootstrap, to provide styling and theming to all Avenue Code products

# Installation
- Install as a npm dependency `npm i git+ssh://git@gitlab.com:acbr/internal/ac-ui/design-system.git`
- 
- Use within your SCSS 
    - Want settings, mixins, extends, with no classes? 
        - `@import "~@ac-design/design-system/src/required";`
    - Want access to Bootstrap's grid classes?
        - No need to import the `required` partial!
        - `@import "~@ac-design/design-system/src/bootstrap/grid";`
