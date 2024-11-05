<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This is a counter that takes a 10K Hz clock as input. Using a divider, I reduce it to a 1 Hz clock,
which is then used as input to a 4-bit counter. The counter's output is passed through a decoder to
map it to hexadecimal numbers (0-F) for display on an LCD screen.

## How to test

My design only uses input 1 and input 2. Setting input 1 to high will stop the clock,
so the counter will stop. Setting input 2 to high will reset the counter to zero.
Then, if we set input 2 to low while input 1 is low, the counter will start.

## External hardware

We need the TinyTapeout design kit to test our circuit.
