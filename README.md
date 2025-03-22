# LED Intensity Controller Based on Ambient Light

This Arduino project adjusts the brightness of an LED based on the surrounding light intensity using an LDR (Light Dependent Resistor). The LED automatically dims in bright conditions and brightens in the dark.

## Components Required
- Arduino Board
- LDR (Light Dependent Resistor)
- 10kΩ Resistor (Pull-down for LDR)
- LED
- Connecting Wires

## Circuit Diagram
### Connections:
- **LDR**: One leg to **5V**, the other leg to **A0** with a 10kΩ pull-down resistor to GND.
- **LED**: Positive (Anode) to **PWM pin (D9)**, Negative (Cathode) to **GND**.


## How It Works
1. **Reads the LDR value** (0-1023) from the analog pin.
2. **Maps the value inversely** (i.e., more light → dim LED, less light → bright LED).
3. **Uses `analogWrite()`** to control LED brightness using PWM.
4. **Displays real-time values** in the Serial Monitor.

## How to Use
1. Connect the components as per the circuit diagram.
2. Upload the provided code to your Arduino board.
3. Open the Serial Monitor (`9600 baud`) to observe real-time readings.
4. Observe how the LED brightness changes based on ambient light.

## License
This project is open-source. Feel free to modify and improve it.

--
