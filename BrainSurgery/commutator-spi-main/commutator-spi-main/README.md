# Torque-free SPI Commutator

The wide-spread availability of 6 degree of freedom pose tracking using internal-measurement units
(IMUs) allows continuous monitoring of an animal's rotational state in an environment. This obviates
the need for tether torque measurements to drive an active commutator since the rotational state of
the animal is known in real-time, and the commutator can simply follow along. This commutator
supports SPI tethers i.e. any headstage that connects to the [standard 12-conductor SPI
cables](https://intantech.com/RHD_SPI_cables.html) with Omnetics connectors.

![Zero-torque coaxial commutator.](./resources/demo.gif)

This commutator functions with headstages that can provide orientation data over SPI. It can also be
used with SPI headstages without an IMU, e.g. using video-based rotation tracking since its remote
control interface is agnostic to how rotational measurements are taken.

For more information, visit the [commutator docs](https://open-ephys.github.io/commutator-docs/).

## Bill of Materials (BOM)

The following BOM pertains to the commutator's mechanical design. You can find the electronics BOM in the [commutator-controller repo](https://github.com/open-ephys/commutator-controller/tree/main/pcb/manufacturing/bom).

| Qty. | Part | Part No. | Description | Link |
| --- | --- | --- | --- | --- |
| 1	| Slip Ring Rotary Joint | Custom part from Orbex | 12-channel Slip Ring with Omnetic Connectors | - |
| 1 | NEMA 11 motor | 11HS18-0674S | 45mm length, 1.8 deg step angle, ~600mA max | [link](https://www.omc-stepperonline.com/nema-11-bipolar-1-8deg-9-5ncm-13-5oz-in-0-67a-4-6v-28x28x45mm-4-wires-11hs18-0674s) |
| 1 | 3D printed case | Custom part | 3D printed | [link](https://github.com/open-ephys/commutator-spi/tree/main/mechanical/production) |
| 1 | 3D printed motor gear | Custom part | 3D printed | [link](https://github.com/open-ephys/commutator-spi/tree/main/mechanical/production) | 
| 1 | 3D printed commutator gear | Custom part | 3D printed | [link](https://github.com/open-ephys/commutator-spi/tree/main/mechanical/production) | 
| 3 | M5 x 8mm socket head cap screws | 91290A224 | for attaching rotary joint to case | [link](https://www.mcmaster.com/91290A224) |
| 4 | M2.5 x 8mm socket head cap screws | 91290A102 | for attaching motor to case | [link](https://www.mcmaster.com/91290A102) |
| 4 | M2.5 x 8mm button head screws | 91239A756 | for attaching PCB to the case | [link](https://www.mcmaster.com/91239A756) |
| 1 | Control PCB | - | - | [link](https://github.com/open-ephys/commutators/tree/main/pcb/manufacturing/gerber) |
| 1 | eBOM | - | electrical components for assembling the PCB | [link](https://github.com/open-ephys/commutators/blob/main/pcb/manufacturing/bom/oe-commutator-controller.html) |
