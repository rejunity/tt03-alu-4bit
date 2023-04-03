![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg)

# Digital design 4-bit ALU. Submission for Tiny Tapeout 03.

This is a digital design for a 4-bit ALU inspired by Z80 and 6502.
I wanted this design to be visually easy to understand, check it out on Wokwi: https://wokwi.com/projects/360745091952588801

## How does it work?

Each clock cycles ALU performs one of the 8 possible operations and stores result in the 4-bit accumulator register.
  accumulator <4 bit> = accumulator <4 bit> (operation) operand <4 bit>

Supported operations:
  lda imm   ::  imm -> accumulator
  neg imm   ::  0x0F - imm -> accumulator
  shr       ::  accumulator / 2 -> accumulator
  sub imm   ::  accumulator - imm -> accumulator
  and imm   ::  accumulator & imm -> accumulator
  xor imm   ::  accumulator ^ imm -> accumulator
  or  imm   ::  accumulator | imm -> accumulator
  add imm   ::  accumulator + imm -> accumulator

## TODO
* Share GDS on Twitter, tag it [#tinytapeout](https://twitter.com/hashtag/tinytapeout?src=hashtag_click) and [link Matt Venn](https://twitter.com/matthewvenn)!
* Explain ALU design with a high-level diagram, include in this README
* Add Negative, Overflow and Zero flag support
* Figure out tidier implementation for hex-to-7segment decoder, probably using ESP32

## What is Tiny Tapeout?

TinyTapeout is an educational project that aims to make it easier and cheaper than ever to get your digital designs manufactured on a real chip!
Go to https://tinytapeout.com for instructions!

## Resources

* [FAQ](https://tinytapeout.com/faq/)
* [Digital design lessons](https://tinytapeout.com/digital_design/)
* [Learn how semiconductors work](https://tinytapeout.com/siliwiz/)
* [Join the community](https://discord.gg/rPK2nSjxy8)

