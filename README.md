![](../../workflows/wokwi/badge.svg)

# Shiftregister 8 Bit

## TinyTapeout

This repository contains a mikrochip design done for TinyTapeout.
Go to https://tinytapeout.com for more informations.

The design is included on the SKY130 shuttlerun MPW-7 with the TinyTapeout project:
https://github.com/mattvenn/tinytapeout-mpw7
https://platform.efabless.com/projects/shuttle_11

## Wokwi project

https://wokwi.com/projects/341506274933867090

## Information about the design

author:       "Thorsten Knoll"

title:        "Shiftregister 8 Bit"

description:  "A simple shiftregister with 8 bit depth, made from D-FlipFlops. Programmable with data and clk, reset. All 8 bits will be mapped to the output."

how_it_works: "Programm the shiftregister with the data (IN0) and clk (IN1) inputs. With reset enabled, the FlipFlops will be cleared with the next rising edge on the clk. The outputs (OUT0 - OUT7) are driven by the shiftregister bits."

how_to_test:  "Each rising edge at the clk input pushs a new data bit into the reǵister. Reset happens with the next clk. See the complete state of the register at the 8 outputs."

external_hw:  "A dipswitch and two button for the inputs. 8 LEDs connected to the outputs."

language:     "wokwi"

wokwi_id:     341506274933867090

picture:      
<img src=shiftregister.png>
<img src=shiftregister_gds_render.png>

inputs:         
  - clock
  - reset
  - none
  - none
  - none
  - none
  - none
  - none

outputs:
  - segment a
  - segment b
  - segment c
  - segment d
  - segment e
  - segment f
  - segment g
  - none
