# Nano-2-4s-AM32-ESC

![License](https://img.shields.io/badge/license-GNU_v3-green.svg)
![Alka motor 32](https://img.shields.io/badge/Firmwire-AM32-red)
![pcb](https://img.shields.io/badge/ESC-v1.1-blue)
![in Volt](https://img.shields.io/badge/20A-2~4S-cyan)


# Specification

* Firmwire: AlkaMotor32(AM32) 

* ESC: 4in1

* MCU: Artery AT32F421 120MHz(QFN28)

* Mosfet: AONR36366

* Gate Driver: DRV8300DRGER(QFN24)

* Input voltage: 2-4s (7.4-16.8v)

* Output current: ~20A (25A brust for 5s)

* mounting size: 25mm*25mm

* mounting pattern: angled/+

* MCU 3.3V? : Onboard buck converter(MP2451DT)

* Current sensing: INA180A with 1mOhm Shunt



# Why 2-4s Nano ESC?
Nano ESC is an open-source ESC hardware design provided by the Alka_Motor_32 project. It can be self-replicated with only some soldering, firmware uploading skills, which the majority of DIY hobiest already have. A conventional 4in1 20A esc costs around 35-50$ with outdated firmware. But if you build Nano 2-4s AM32 ESC, you can get 5 ESCs at ~110$ that only costing around 25$ each. Also, as you are building it, it would be very easy to fix one if damaged.

# Documentations
In this repository, you can find the Schematics, Gerber file, pick and place(if you plan to use PCBA from PCB manufacturer), and all the components you need(aka BOM) files, along with all the steps to build your own 4-in-1 20A ESC. Also, if you want to make a full custom 3s 3ich drone with this ESC then checkout [HACK-FLY-32](https://github.com/minhazislamnafi/HACK-FLY-32).

# Quick Start

## Requirements

## Components:

* MCU: Artery AT32F421G8U7 120MHz QFN-28 (4 pcs) [link](https://s.click.aliexpress.com/e/_c4PMPWk9)
* Mosfet: AONR36366 QFN-8 package (24 pcs) [link](https://s.click.aliexpress.com/e/_c3cixcnL)
* Gate driver: DRV8300DRGER QFN-24 (4 pcs) [link](https://s.click.aliexpress.com/e/_c3NqUJhL)
* 3.3v buck: Mp1584EN soic-8 [link](https://s.click.aliexpress.com/e/_c3PCEJ6N) (recommended to buy a buck module and harvest all the necessary components, rather than buying the inductor, resistor, and diodes separately)
* current sense: INA180IDBVR [link](https://s.click.aliexpress.com/e/_c3yf2AqD)
* Shunt: 2512 3W R001 1MR [Link](https://www.aliexpress.com/item/1005010000851939.html?)
* Resistors: 10k, 1k, 10r etc 0402 size [link](https://s.click.aliexpress.com/e/_c4mdiRd3)
* Capacitors: 10uf, 1uf, 100nf, etc 0402 size [Link](https://s.click.aliexpress.com/e/_c3HHiS9r)




