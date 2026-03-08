# cosmic-alpental-theme

Alpental dark and light themes for Cosmic Desktop Environment.

## Usage

Use the import option in **Settings → Desktop → Desktop Options → Window Appearance** to load `themes/Alpental-Dark.ron` or `themes/Alpental-Light.ron`.

## Prerequisites

- Install the [veneer-theme](https://github.com/ascarter/veneer-theme) CLI used to build the theme assets:
  ```sh
  cargo install --git https://github.com/ascarter/veneer-theme
  ```
- Install [just](https://just.systems) for running the task recipes:
  ```sh
  brew install just
  ```

## Build

Generate the compiled theme files:

```sh
just build
```

The output ends up in `themes/` as `Alpental-Dark.ron` and `Alpental-Light.ron`.

## Design

Alpental is built around a high-usability palette principle: UI chrome stays neutral and achromatic, with color reserved strictly for semantic meaning (errors, warnings, success states). The accent color is a neutral gray to avoid COSMIC's hardwired use of `accent` for selected text and focus indicators bleeding chromatic color into everyday interface elements.
