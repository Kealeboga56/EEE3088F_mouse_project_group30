# EEE3088F Micro-mouse Sensing Subsystem

This repository contains the design files and documentation for the sensing subsystem of the EEE3088F Micro-mouse project.

## Design Files

The design files for the sensing subsystem PCB were created using KiCad EDA. The schematic and PCB layout files are located in the `sensing` directory.

## Footprint Import

To import footprints from EasyEDA into KiCad, the `easyeda2kicad` Python script was used. This script converts the EasyEDA footprint files to the KiCad format, allowing for seamless integration of components from the EasyEDA library into the KiCad project.

The `easyeda2kicad` script can be found at [https://pypi.org/project/easyeda2kicad/](https://pypi.org/project/easyeda2kicad/).

To use the script, follow these steps:

1. Install the required dependencies (`lxml` and `click`) by running `pip install easyeda2kicad` in your terminal.
2. Run the script with the appropriate arguments, specifying the input EasyEDA footprint file and the output directory for the KiCad footprint files.more on how to use it at [https://pypi.org/project/easyeda2kicad/]
