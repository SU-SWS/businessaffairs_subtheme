# Business Affairs Subtheme

A Stanford Sites subtheme for Stanford Business Affairs, built on the `stanford_basic` base theme and scaffolded from `stanford_starter`.

## Version

1.x

## Setup

1. `cd businessaffairs_subtheme`
2. `npm install` (or `yarn install`)
3. `npm run build` to compile CSS, or `npm run watch` for development.

## SCSS Structure

```
src/scss/
├── main.scss                  # Entry point — imports everything
├── ckeditor5.scss             # CKEditor 5 editor styles
├── utilities/
│   ├── index.scss
│   ├── variables/
│   │   ├── index.scss
│   │   └── _colors.scss      # BA-specific color variables ($ba-color-*)
│   └── mixins/
│       ├── index.scss
│       ├── _buttons.scss     # Button mixins (ba-button-*)
│       ├── _cta.scss         # CTA/link mixins (ba-cta-*)
│       └── _link-icon.scss   # Decanter icon color helpers
├── base/index.scss            # HTML element styles only (no classes)
├── components/index.scss      # Discrete, reusable UI components
├── layout/index.scss          # Page/grid layout
├── state/index.scss           # Client-side state (.is-*, js-*)
├── print/index.scss           # Print styles
└── theme/
    ├── index.scss
    ├── _button.scss           # Button look-and-feel overrides
    └── _cta.scss              # CTA/link look-and-feel overrides
```

## Naming Conventions

- SCSS variables: `$ba-color-[name]`
- SCSS mixins: `ba-[mixin-name]`
- CSS classes: `.ba-[component-name]`
