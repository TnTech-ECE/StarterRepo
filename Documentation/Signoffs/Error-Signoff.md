Reference link: https://www.ti.com/solution/professional-microphones-wireless-systems?variantid=34929&subsystemid=18462
# Error Subsystem

## Function of the Subsystem
The goal of this subsystem is to input the acoustic audio from the room, amplify the audio to a workable signal, modulate the signal to a radio frequency, and broadcast the signal to the Bluetooth receiver subsystem.
## Constraints
### The transmitted signal shall operate on Bluetooth frequencies (2.4 GHz). Origin: Bluetooth subsystem requirements
The Bluetooth subsytem is designed to accept frequencies operating at Bluetooth frequencies, so the transmission must match that.
Bluetooth is commonly used to wirelessly transmit signals. These kinds of transmissions typically work in a point-to-point manner at a low-power cost. Also, the FCC is subject to change what frequencies wireless microphones are allowed the transmit at [1]. For these reasons, Bluetooth is ideal for long-term use. 

### The transmitter must be powered with a wall outlet. Origin: Device requirements
Using an electret microphone will allow the microphone to work without power, but the transmitter requires power to operate at the lengths the main device will be operating at. The main processor requires an error signal to properly calculate its outputs, so without an error signal, the main device cannot function properly.

## Buildable Schematic
<img src="https://user-images.githubusercontent.com/123997954/229912784-1174c224-1c0f-4fb9-8a78-3f503ecb81d3.png" width="60%" height="60%">
![Image](https://github.com/CarsonDPope/Active-Noise-Control-With-Wall-Transmission-Detection/blob/jmvega42-Error-Signoff/Documentation/Images/Error/OVC3868_Pins.jpg?raw=true)
## Analysis

Include math of frequency modulation here

## BOM
| DEVICE                                       | Quantity | Price Per Unit | Total Price |
|----------------------------------------------|----------|----------------|-------------|
| OVC3860 Bluetooth Transmitter [2] [3] | 1 | $7.55 | $7.55 | 
| Simple Microphone [4] | 1 | $8.99 | 8.99|

References 2 and 3 are options for the transmitter. 3 Shows a simplified version while 2 has the chip uncased.

## References
[1] “Operation of Wireless Microphones.” Www.fcc.gov, 15 Oct. 2019, www.fcc.gov/consumers/guides/operation-wireless-microphones. Accessed 16 Apr. 2023.

[2] https://soldered.com/product/bluetooth-audio-module-ovc3860/

[3] https://www.amazon.com/Bluetooth-Backplane-Adapter-OVC3860-Voltage/dp/B09W367VDC

[4] https://www.amazon.com/Phone-Microphone-Headphone-Jack-Detachable/dp/B07SNSY64C/ref=sr_1_2?crid=2MBJ9LDPPDAEA&keywords=microphone+jack&qid=1681674869&sprefix=microphone+jack%2Caps%2C90&sr=8-2

### Ignore
OPA1692—SoundPlus™ Low-Power, Low-Noise, High-Performance Dual Bipolar-Input Audio Op Amp
https://www.ti.com/lit/ds/symlink/opa1692.pdf?ts=1681613780693&ref_url=https%253A%252F%252Fwww.ti.com%252Fsolution%252Fprofessional-microphones-wireless-systems%253Fvariantid%253D34929%2526subsystemid%253D18462

LMX2694-EP
found here: https://www.ti.com/rf-microwave/rf-plls-synthesizers/products.html
https://www.ti.com/lit/ds/symlink/lmx2694-ep.pdf?ts=1681614207711&ref_url=https%253A%252F%252Fwww.ti.com%252Frf-microwave%252Frf-plls-synthesizers%252Fproducts.html


[2] https://www.tinyosshop.com/index.php?route=product/product&path=158&product_id=1090

[3] https://tinkersphere.com/audio/3639-bluetooth-audio-transmitter-receiver.html