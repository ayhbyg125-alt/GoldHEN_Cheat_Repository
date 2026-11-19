# FN Menu Hider — Rectangle Profile

This repository entry documents the visual rectangle configuration used by the Fortnite Menu Hider GoldHEN plugin.

## Controls

- L1 + R1: open/close the plugin menu
- L1 + Down: arm/disarm the rectangle
- Up/Down: select an item
- Left/Right: change width/height
- Square: toggle rectangle
- Circle: close
- X: untouched/pass-through

## Default rectangle

- X: 0
- Y: 0
- Width: 320
- Height: 120
- Width range: 32–4096
- Height range: 16–4096
- Step: 16 pixels

## Runtime architecture

The GoldHEN Cheat Menu formats (json, shn, and mc4) are memory-cheat formats. They do not provide a mechanism for loading a PRX or directly invoking the plugin's framebuffer renderer. Therefore this profile is intentionally kept as plugin configuration/documentation rather than pretending to be a functional memory cheat.

The actual rectangle renderer remains in button_swap.prx, where it can safely observe controller state and modify only the framebuffer.

Target title: CUSA07669.
