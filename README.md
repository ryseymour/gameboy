# 8 Bit Astronaut 🚀

A Game Boy Color homebrew action-platformer, written in C with GBDK 2020. Mine procedurally generated asteroids, manage your oxygen and fuel, and fight through hostile alien factions, all running on real Game Boy hardware (and in your browser, below).

## ▶ Play it in your browser
**[ryseymour.github.io/gameboy](https://ryseymour.github.io/gameboy/)**

No install needed. The page runs the actual compiled Game Boy ROM on a WebAssembly emulator.

## About the game
- **Procedurally generated levels:** every asteroid is carved fresh, with ore, hazards, and enemies placed by a seed-driven generator, so no two runs are the same.
- **Resource management:** balance oxygen and jetpack fuel as you dig deeper and the danger rises.
- **Physics-based combat:** a pickaxe melee plus a downward plunge / pogo move for bouncing off and chaining hits on enemies.
- **Multiple enemy factions,** each with its own behavior and escalation.

## Controls (Game Boy buttons)
- **D-pad:** move
- **A:** jump / jetpack
- **B:** swing pickaxe / attack
- **Start:** menus

The browser emulator maps these to your keyboard; the mapping is shown on the play page.

## Tech
- Written in **C** with **GBDK 2020 / SDCC**, targeting MBC5 (Game Boy Color). Runs on original hardware.
- This repository is the **web build**: the compiled ROM (`rom/game.gb`) bundled with a WebAssembly Game Boy emulator so the game can be played in any modern browser.

## Credits & license
The in-browser emulator is **[binjgb](https://github.com/binji/binjgb)** by Ben Smith (binji), used under the MIT License (including changes from community forks for GB Studio support). All emulator credit goes to its authors. The 8 Bit Astronaut game itself is © Ryan Seymour.

binjgb MIT License notice:

> Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND.
