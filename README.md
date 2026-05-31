# Nano-2-4s-AM32-ESC

![License](https://img.shields.io/badge/license-OHL_v2-green.svg)
![Alka motor 32](https://img.shields.io/badge/Firmwire-AM32-red)
![pcb](https://img.shields.io/badge/ESC-v1.1-blue)
![in Volt](https://img.shields.io/badge/20A-2~4S-cyan)

<img width="4000" height="5657" alt="2-4s nano esc" src="https://github.com/user-attachments/assets/405818a3-915a-408f-9ea7-05be12fab259" />



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

## For detailed part list, price, and values checkout [BOM](https://github.com/minhazislamnafi/Nano-2-4s-AM32-ESC/blob/main/BOM.csv)

## PCB
Use JLCPCB if you're in ASIA or PCBWAY if you're in America. Also, find what manufacturer is better for you. 
If you just want to get Flight controller PCB then use this [GARBER file](https://github.com/minhazislamnafi/Nano-2-4s-AM32-ESC/blob/main/PCB/Gerber_PCB_Nano-2-3s-AM32-ESC_r1.zip),Download it and place order.
Or if you just want to build your own PCB, then follow this [SCHEMATICS](https://github.com/minhazislamnafi/Nano-2-4s-AM32-ESC/blob/main/PCB/SCH_Nano%202-3s%20AM32%20ESC_2026-05-22.pdf).

## 6 Layers
<img width="1672" height="2400" alt="6 layer 2-Photoroom" src="https://github.com/user-attachments/assets/5757c659-2350-404c-82b6-b7f7b7d1450e" />

## PCB render
<img width="2400" height="1167" alt="ESC bg-Photoroom" src="https://github.com/user-attachments/assets/d0983aa1-ba67-49ca-bbfa-9ce00b8f2a9c" />

## FOLLOW THESE STEPS ##

**1. Spend some money $$ to buy the parts mentioned in [BOM](https://github.com/minhazislamnafi/Nano-2-4s-AM32-ESC/blob/main/BOM.csv).**

**2. Order the Nano ESC PCB using this [GERBER file](https://github.com/minhazislamnafi/Nano-2-4s-AM32-ESC/blob/main/PCB/Gerber_PCB_Nano-2-3s-AM32-ESC_r1.zip).**

**3. Solder the SMD components of the PCB by hand ;) Or just order the PCBs with PCBA services, btw it will cost a lot.**

**4. solder 18 AWG wire with xt30 connector.**

**5. Check with multimeter- Is mcu getting 3.3v or not, if not diagnose by yourself :)**

**6. Flash each mcu with AM32 firmware using Stlink v2 programer ( I will add every step in details, once I have built IRL:)**





