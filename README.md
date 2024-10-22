# POE Pico
"POE Pico" is a PCBA design for a RP2040 "Pi Pico" configured to support 40W active POE with Ethernet <-> USB conversion. 
# Diagram
Pre-print, the following 3D Views are available, but are not fully representative of the final product:
<br />Top<br />
<a href="https://ibb.co/r2JVWjt"><img src="https://i.ibb.co/yFJr39R/3-Dview-Top.png" alt="3-Dview-Top" border="0"></a>
<br />Bottom<br />
<a href="https://ibb.co/tpYNBwX"><img src="https://i.ibb.co/4R4DWwd/3-DView-Bot.png" alt="3-DView-Bot" border="0"></a>

A PDF export of the schematic sheets for reference can be found [here](documentation/POEPico.pdf).
# Feature List
## Components
The USB to Ethernet conversion IC is a [LAN9500A](https://www.microchip.com/en-us/product/lan9500a). The board features a 40W active POE power/data supply input with a fully-isolated 12 VDC @ 2A Flyback courtesy of an [LT4295](https://www.analog.com/media/en/technical-documentation/data-sheets/LT4295.pdf). Downstream of the flyback is a 12V to 5V buck converter and 3.3V power rails. Ethernet magnetics and LEDs are fully integrated by the RJ45 connector. 

Alternatively, the board supports bringup of the RP2040 and power through the Micro-B connector. Powering the PCBA through the 5V Micro-B connector will also power the 3.3V rail. 
## Pins
Header pins expose standard RP2040 GPIO, including an isolated 12V, 5V, and 3.3V power rail.
| Purpose | Pin | Pin | Purpose | 
| -------- | ------- | ------- | ------- |
| GND | J21.1 | J21.2 | +3V3 |
| GND | J21.3 | J21.4 | GPIO0 |
| GND | J21.5 | J21.6 | GPIO1 |
| GND | J21.7 | J21.8 | GPIO2 |
| GND | J21.9 | J21.10 | GPIO3 |
| GND | J21.11 | J21.12 | GPIO4 |
| GND | J21.13 | J21.14 | GPIO5 |
| GND | J21.15 | J21.16 | GPIO6 |
| GND | J21.17 | J21.18 | GPIO7 |
| GND | J21.19 | J21.20 | GPIO8 |
| GND | J21.21 | J21.22 | GPIO9 |
| GND | J21.23 | J21.24 | GPIO10 |
| GND | J21.25 | J21.26 | GPIO11 |
| GND | J21.27 | J21.28 | GPIO12 |
| GND | J21.29 | J21.30 | GPIO13 |
| GND | J21.31 | J21.32 | GPIO14 |
| GND | J21.33 | J21.34 | GPIO15 |
| GND | J21.35 | J21.36 | +5V0 |

| Purpose | Pin | Pin | Purpose |
| -------- | ------- | ------- | ------- |
| SWCLK | J22.1 | J22.2 | GND |
| SWD | J22.3 | J22.4 | GND |
| RUN | J22.5 | J22.6 | GND |
| GPIO16 | J22.7 | J22.8 | GND |
| GPIO17 | J22.9 | J22.10 | GND |
| GPIO18 | J22.11 | J22.12 | GND |
| GPIO19 | J22.13 | J22.14 | GND |
| GPIO20 | J22.15 | J22.16 | GND |
| GPIO21 | J22.17 | J22.18 | GND |
| GPIO22 | J22.19 | J22.20 | GND |
| GPIO23 | J22.21 | J22.22 | GND |
| GPIO24 | J22.23 | J22.24 | GND |
| GPIO25 | J22.25 | J22.26 | GND |
| GPIO26 | J22.27 | J22.28 | GND |
| GPIO27 | J22.29 | J22.30 | GND |
| GPIO28 | J22.31 | J22.32 | GND |
| GPIO29 | J22.33 | J22.34 | GND |
| +12V0 | J22.35 | J22.26 | GND |

# Assembly
To be assembled as a 4-layer PCB, with associated BOM. Components to be placed on top and bottom of board. BOM has been edited to support JLCPCB quoting. Approximate cost estimate as of 21/10/2024 is $60/pc, including fabrication, components, assembly, and shipping.

