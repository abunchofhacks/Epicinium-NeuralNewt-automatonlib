# Epicinium NeuralNewt automaton library

Library and header files for the [Epicinium](https://epicinium.nl) automaton,
which implements Epicinium's game logic to calculate subsequent game states.

Dependency for [Epicinium-NeuralNewt](https://github.com/abunchofhacks/Epicinium-NeuralNewt),
a framework for training neural networks to play Epicinium with evolutionary training techniques.

Source files for this library can be found in the
[Epicinium-lib-rs repository](https://github.com/abunchofhacks/Epicinium-lib-rs).
It can be compiled with `make automatonlib` in its `epicinium` folder.
Before doing so, you might want to edit the following constants
to correspond with the header files in this repository:
- In `position.hpp`, `MAX_COLS = 20` and `MAX_ROWS = 13`
- In `tiletype.hpp`, `TILETYPE_SIZE = 19`
- In `unittype.hpp`, `UNITTYPE_SIZE = 8`

We decreased these variables to shrink the input space for NeuralNewt
and thus make learning easier.
Sorry for these confusing references - 
we plan to set this up better sometime, since:

The rest of Epicinium will be open-sourced in the near future.
It will also be coming soon to [Steam](https://epicinium.nl/steam).

Epicinium is being developed by [A Bunch of Hacks](https://abunchofhacks.coop),
a worker cooperative for video game and software development from the Netherlands.
Contact us at [info@epicinium.nl](mailto:info@epicinium.nl).

## Contents

* `bin/epicinium-automaton.a`, a library implementing the latest Epicinium automaton compiled for 64-bit Linux (Debian-based).
* `bin/epicinium-automaton.lib`, a library implementing the latest Epicinium automaton compiled for 64-bit Windows.
* In `include/`, header files for the classes and methods implemented by this library.

## License

The Epicinium NeuralNewt automaton library
was created by [A Bunch of Hacks](https://abunchofhacks.coop).
It is made available to you under the AGPL-3.0 License,
as specified in `LICENSE.txt`.

This library is free software; you can redistribute it and/or modify it under the terms of the GNU Affero General Public License (AGPL) as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

## Related repositories

*  [Epicinium documentation](https://github.com/abunchofhacks/epicinium-documentation), which includes a wiki and a tutorial for Epicinium
*  [Epicinium-NeuralNewt](https://github.com/abunchofhacks/Epicinium-NeuralNewt), a libtorch framework for training neural networks to play Epicinium via NeuralNewt, a parameterized decision tree AI, with evolutionary training techniques
*  [Epicinium-lib-rs](https://github.com/abunchofhacks/Epicinium-NeuralNewt-automatonlib), Rust bindings for libepicinium, the game logic library of Epicinium