Relay Toggle Circuit Using a 555 Timer

Description
This 555 timer circuit below toggles a relay when a button is pressed. Pins 2 and 6, the threshold and trigger inputs, are held at 1/2 the supply voltage by the two 10K resistors. When the output is high, the capacitor charges through the 100K resistor, and discharges when the output is low. When the button is pressed, the capacitor voltage is applied to pins 2 and 6 which causes the output to change to the opposite state. When the button is released, the capacitor will charge or discharge to the new level at the output (pin 3). The parts are not critical, the resistors can be somewhat higher or lower, but the 2 resistors at pins 2 and 6 should be equal values, and the resistor connected to the cap should be 10 times greater or more.

![image](https://github.com/user-attachments/assets/4f5b1d8b-144d-44da-acdd-ff2314be13fd)

Advantages of this circuit are the large hystersis range at the input which avoids false triggering, and only a few parts are needed for construction. One disadvantage is the relay may be engaged when power is first applied. To solve this problem, you could tie the reset line (pin 4) to another resistor/capacitor combination with the capacitor at ground and the resistor at the +V point. This will cause pin 4 to be held near ground for a short period which will reset the output when power is applied.

The 100 ohm resistor and 100uF capacitor serve to filter noise on the supply line if the circuit is used in a automotive application. They may not be necessary. The circuit may work well without those parts.
