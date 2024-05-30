# Wokwi cd4068b Chip

This is a custom chip for [Wokwi](https://wokwi.com/). It implements the cd4068b IC.

## Description

The cd4068b contains 8 input nand/and gate . It performs the Boolean functions
of :
- J = NOT( A . B . C . D . . E . F . G . H ) .
- K = ( A . B . C . D . . E . F . G . H ) .

## Pin names

| Name | Description        |
| ---- | ------------------ |
|  A   | Input signal  A    |
|  B   | Input signal  B    |
|  C   | Input signal  C    |
|  D   | Input signal  D    |
|  E   | Input signal  E    |
|  F   | Input signal  F    |
|  G   | Input signal  G    |
|  H   | Input signal  H    |
|  J   | Output signal NAND |
|  K   | Output signal AND  |
| GND  | Ground             |
| VCC  | Supply voltage     |


## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-cd4068b": "github:wokwi-custom-chips/cd4068b@0.1.0"
  }
```

Then, add the chip to your circuit by adding a `chip-cd4068b` item to the `parts` section of diagram.json:

```json
  "parts": {
    ...,
    { "type": "chip-cd4068b", "id": "chip1" }
  },
```

For a complete example, see [The cd4068b chip test project](https://wokwi.com/projects/399335684070736897).
