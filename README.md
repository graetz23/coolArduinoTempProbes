## cool Arduino Temperature Probes

### Introduction
cool Arduino Temperature Probes (coolATP) drives Negative (\& poitive) Temperature Coefficient (NTC) probes on all available _analog inputs_ and makes resistor values in _Ohm_ or the temperature in _K_, _°C_, or _°F_ available.

### Building
For building the HEX file, the [arduino Makefile](https://github.com/sudar/Arduino-Makefile) is used. So clone or download / unzip this first to your system. Afterwards configure the _Makefile_ to your arduino boards and type: _make_.

### Hardware
Wire your NTC probe with a _matching_ (same resistor value as the probe) resistor in series. Wire from the mid (between your probe and your resistor) of this _voltage divider_ to an _ananlog_ input of your arduino. Wire the _5 V_ (not system's volatage - there are two _5 V_ voltage sources) and GND to the ends of your _voltage divider_.

However there are several public _posts_, _blogs_, and _vlogs_ on internet showing a schematic wiring diagram.

### Usage
See [coolATP.ino](https://github.com/graetz23/coolArduinoTempProbes/blob/master/coolATCP.ino) file as an example.

### Remarks
I use this project for driving several NTCs in a home brewery system and using [**ASSTP**](https://github.com/graetz23/coolArduinoSerialStateTempPrbes) to transfer data via serial to a _raspberry pi_. The pi is driving  [**CraftBeerPi3**](https://github.com/Manuel83/craftbeerpi3) by a written plugin, to integrate the temperature values: [craftbeerpi3ArduinoTempProbes](https://github.com/graetz23/craftbeerpi3ArduinoTempProbes).

Everything was coded using:

  - [**atom**](https://atom.io/) editor,
  - [**arduino Makefile**](https://github.com/sudar/Arduino-Makefile),
  - [**Gnome**](https://www.gnome.org/) windows manager,
  - and [**debian**](https://www.debian.org/) GNU/Linux.

## ChangeLog

**20200405**
  - renamed project and reposiory,
  - updated readme

**20200331**
  - adding MIT License to all files.
  - adding the README.md for explanation,
  - setting up reository on [github.com](https://github.com/graetz23/coolArduinoTempProbes).
