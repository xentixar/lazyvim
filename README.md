# 💤 LazyVim + Laravel

(and some stuff I also use)
This is my best effort to fully integrate my LazyVim config with Laravel and all Laravel-related tools.
Works great with Livewire v3 as well as Volt and Folio.
When using Volt, use class-based syntax for maximum compatibility.
Functional Volt works, too, but has issues with `$this`.

A starter template for [LazyVim](https://github.com/LazyVim/LazyVim).
Refer to the [documentation](https://lazyvim.github.io/installation) to get started.

## Laravel Native

This config is setup with the best available dev tooling for laravel

- Intelephense
- Blade Language Support
- Blade Formatter
- Pint
- Phpstan (make sure you configure larastan in your project)
- Rustywind
- Tailwind LS
- XDebug with configuration for Laravel Sail

## Additions

### Requirements

If you encounter an issue with `Intelephense` not recognising facade or model function calls, you will need to install [Laravel IDE Helper](https://github.com/barryvdh/laravel-ide-helper) into your project and execute the relevant artisan commands. Thanks to [@ermand](https://github.com/ermand) for bringing up the issue as well as the solution.

Optional:

- lazygit
- lazydocker

(you should use both, they are great)

### LSP

- Tailwind support
- Intelephense for php (best in class for Laravel development)

### Formatting

- Eslintd for when an `.eslintrc.json` is found (use the eslint prettier plugin for best performance and compatibility)
- Tailwind color preview

### Theme

- Changed to gruvbox

## Troubleshooting

If opening a py file leads to pyright analyzing your whole library, make sure to add an empty `pyrightconfig.json` into the file root.
This can be your $HOME folder or for example on darwin using homebrew it could be `/opt/homebrew/`.
