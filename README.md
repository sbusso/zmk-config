## Getting started

      · Change buildSplitKeyboard to buildKeyboard in
        flake.nix if not using a split keyboard
      · Edit for the desired ZMK board and shield(s) in
        flake.nix
      · Create and edit config/<shield>.conf and
        config/<shield>.keymap to your liking
      · Run nix run .#flash to flash firmware

## Maintenance

      · Run nix run .#update to update West dependencies,
        including ZMK version, and bump the zephyrDepsHash on
        the derivation
      · GitHub Actions to automatically PR flake lockfile
        bumps and West dependency bumps are included
      · Using something like Mergify to automatically merge
        these PRs is recommended - see
        https://github.com/lilyinstarlight/zmk-nix/blob/main/.github/mergify.yml
        for an example Mergify configuration
