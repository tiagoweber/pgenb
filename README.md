# PGEN-B: PWL Voltage Generator from Bitstream

This program was created to help circuit designers have a quick and easy way to generate PWL (Piece-Wise Linear) voltage sources from bitstreams to use in SPICE simulators (such as NGspice).

SPICE simulators such as NGSPICE have no native way of describing digital voltage sources from bitstreams. Therefore, if you want to create a voltage source that behaves like a bitstream, you need to create a PWL source. Although simple to create, these PWL sources require a time and voltage pair for each point in the waveform. If you take into account the rise and fall time of the waveform, this mounts up quickly in number of points. Additionally, if you have to change the bitstream, creating it again or modifying it may be a hassle. Therefore I created this simple and easy to use PWL waveform generator.

It outputs code that can be directly used in NGSPICE for instance.

## Functionalities

- has a waveform preview inside the program;
- exports waveform(s) directly to external file with necessary simulation commands to test it
- copy waveform(s) to clipboard
- allows selecting period, rise/fall time, high and low voltage
- allows the use of parameterized values or the direct use of the calculated ones 
- has the option to use half of the period for describing each bit in the bitstream (useful if you want to test how a system behaves with changes before the rising/falling clock)
- can generate multiple waveforms at once. It also allow comments to be added directly in the generated code.
- allows saving and loading the bitstreams with their comments and options in a config file.

# About the author and license

- Copyright 2025 Tiago Oliveira Weber
- License: MIT License
- Repository: https://github.com/tiagoweber/pgenb
- Author professional website: www.tiagoweber.com.br
- Contact: tiago.oliveira.weber@gmail.com
