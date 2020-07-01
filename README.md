![Jet Propulsion Laboratory, California Institute of Technology (NASA JPL)](Images/Misc/NASA_JPL_LOGO.jpg)
# PULSE - a pendant to warn you when you touch your face
Here’s the tool and equipment list, materials, circuit diagram and assembly instructions. The ability to solder is necessary to assemble the PULSE pendant. Except for the IR sensor unit, the parts are generic and can be purchased broadly. Example links for purchasing these parts are shown.

### Table of Contents
* [Tools and equipment needed](https://github.com/nasa-jpl/Pulse#tools-and-equipment-needed)

* [Materials Required and links for ordering](https://github.com/nasa-jpl/Pulse#materials-required-and-links-for-ordering)

* [Pendant Case](https://github.com/nasa-jpl/Pulse#pendant-case)

* [Circuit Diagram](https://github.com/nasa-jpl/Pulse#circuit-diagram)

* [Assembly of the PULSE pendant](https://github.com/nasa-jpl/Pulse#assembly-of-the-pulse-pendant)

* [DISCLAIMER](https://github.com/nasa-jpl/Pulse#disclaimer)

* [Contact Us](mailto:pulse@jpl.nasa.gov)



### Tools and equipment needed

1.	Home-class 3D Printer (PLA material or other as user option; you can also send files out for on-line order)

2. Soldering Iron and solder

3. Wire Stripper

4. Helping Hands Stand to Assist Soldering (optional)

### Materials Required and links for ordering

![Materials_Required.jpg](Images/Materials_Required.jpg)

1. IR Sensor unit: Pololu 38 kHz IR Proximity Sensor [Order Here](https://www.pololu.com/product/2578)

2. PNP Transistor: 2N3906 or equivalent: [Order Here](https://www.amazon.com/Projects-B-0001-A10f-General-Transistor-92/dp/B07Y3GFR5P/ref=sr_1_6?dchild=1&keywords=2n3906+transistor&qid=1589929461&sr=8-6)

3. 1 K Ohm standard resistor: [Order Here](https://www.amazon.com/EDGELEC-Resistor-Tolerance-Resistance-Optional/dp/B07HDDWFDD?ref_=ast_slp_dp)

4. Slide Switch to fit case: [Order Here](https://www.amazon.com/gp/product/B07NLR444L/ref=ppx_yo_dt_b_asin_title_o06_s00?ie=UTF8&psc=1)

5. Vibrating Motor to fit case [Order 10x2.0mm Vibrating Motor Here](https://www.pololu.com/product/1638) or [Order 10x3.4mm Vibrating Motor Here](https://www.pololu.com/product/1636)

6. W1 – 5 cm; W2 – 4 cm; W3 – 2 cm; W4 – 2 cm; 22 Gage Wire

7. Heat shrink tubing to cover leads: [Order Here](https://www.amazon.com/560PCS-Heat-Shrink-Tubing-Eventronic/dp/B072PCQ2LW/ref=sr_1_5?dchild=1&keywords=shrink+wrap&qid=1589929721&s=industrial&sr=1-5)

8. Battery Holder: [Order Here](https://www.amazon.com/gp/product/B07FL8MFK8/ref=ppx_yo_dt_b_asin_title_o01_s01?ie=UTF8&psc=1)

9. 3V CR2032 Coin Battery: [Order Here](https://www.amazon.com/gp/product/B071D4DKTZ/ref=ppx_yo_dt_b_asin_title_o09_s01?ie=UTF8&psc=1)

10. Dark colored paint (i.e., acrylic, oil, nail polish etc.) such as black, navy blue, dark green, etc. (Required only when utilizing non-black colored case material)
 
### Pendant Case

The PULSE pendant case was designed to hold the existing parts. Other pendant designs can be created as desired as long as the IR sensor will fit and has a clear view to the front of the pendant.
 
If not using black material for case, the bottom of the IR emitter will need to be painted black or covered with black electrical tape to absorb any light. If this is not done, the sensor will read false motion and vibrate continuously. Only the flat bottom, do not cover the whole LED.

[Download STL Files](https://github.com/nasa-jpl/Pulse/tree/master/CAD)

![cad_with_parts.jpg](Images/cad_with_parts.jpg)

### Circuit Diagram

![Circuit_Diagram.jpg](Images/Circuit_Diagram.jpg)

Central to the design of the PULSE pendant is the infrared sensor unit (U1 in the diagram) that provides a high (~3 V) output signal to pin 3 by default, and drops low (~1 V) when the LED detector (D1) receives a signal indicating your hand (or other reflecting object) is in front of the pendant.  L1 is the radiating infrared LED. When pin 3 goes low, it powers the PNP transistor (Q1) to energize the motor (M1) causing it to vibrate and the pendant to pulse. V1 is the 3 V battery in the case and S1 is the slide switch. Pin 4 on the infrared sensor is an enable input and is not used.

### Assembly of the PULSE pendant

1. Wire W1 solders to the center pin of the switch and wire W2 solders to an end pin of the switch. The third pin on the switch can be 		clipped off – it is not used. Heat shrink covers the pins. This picture shows the completed switch next to an assembled PULSE pendant

![assembly_step_1.jpg](Images/assembly_step_1.jpg)

2. The other end of W2 solders to the emitter pin of the transistor as well as wire W3. (This is a three-way connection – wires W2, W3 		and the transistor emitter pin are connected together; this is the positive voltage). The picture shows the use of a helping hands to 	perform the soldering of three leads, and then the end result. Heat shrink is used to cover the lead at the transistor.

![assembly_step_2.jpg](Images/assembly_step_2.jpg)

3. The other end of wire W3 then attaches to pin 2 of the IR sensor

4. Wire W4 (ground), attaches to pin 1 of the IR sensor

5. The 1 K Ohm standard resistor attaches to the middle or base pin of the transistor

6. The 1 K Ohm standard resistor attaches to pin 3 of the IR sensor. This picture shows the assembly so far

![assembly_step_5.jpg](Images/assembly_step_5.jpg)

7. The red wire of the vibrating motor solders to the collector pin of the transistor. Use heat shrink to cover the connection

![assembly_step_6.jpg](Images/assembly_step_6.jpg)

8. The black wire of the vibrating motor solders to the ground port of the battery case (jointly with W4). The other end of W1 solders 		to the positive pin of the battery holder. This picture shows the completed assembly and the wires folded for insertion into the 				bottom case

![assembly_step_7.jpg](Images/assembly_step_7.jpg)

9. The motor and switch snap into the case base

10. The IR sensor slides into the case base rails

11. The electronics are gently tucked into the case base

![assembly_step_10.jpg](Images/assembly_step_10.jpg)

12. Using a dark colored paint (i.e., acrylic, oil, nail polish etc.) such as black, navy blue, dark green, etc., lightly paint over the 		emitter as shown in the image below. Using a dark colored pen or marker will not work the same as paint. 

![assembly_step_11.jpg](Images/assembly_step_11.jpg)

13. With the electronics in the case base, the battery can be installed, the switch can be set on; move your hand in front of the IR 				sensor and the red LED on the sensor board will light and the case will PULSE!  

[![GitHub_Video_Thumbnail.jpg](Images/Misc/GitHub_Video_Thumbnail.jpg)](https://www.youtube.com/watch?v=7utCPXKdKHg&list=PLKWlaxzCh8uKqaNQIiBa6WjCEDBVH6ehV&index=3)

14. Install the top case. Attach a necklace of your choice and PULSE is complete

### DISCLAIMER

DISCLAIMER: The designs herein have not been reviewed, cleared, or approved by FDA or other regulatory authority, nor have they received Coronavirus Disease 2019 (COVID-19) Emergency Use Authorizations for Medical Devices. Neither California Institute of Technology (including the Jet Propulsion Laboratory)("Caltech") nor its employees or agents provide any representation or warranty, express or implied, for fitness for a particular purpose, safety, efficacy, or non-infringement of any third party intellectual property rights. Caltech offers these device designs in good faith to help healthcare providers and others prevent the spread of and treat patients with COVID-19. Physicians and other healthcare providers bear full responsibility to convey warnings and obtain patients' informed consent.

### [Contact Us](mailto:pulse@jpl.nasa.gov)

### The research was carried out at the Jet Propulsion Laboratory, California Institute of Technology, under a contract with the National Aeronautics and Space Administration.
