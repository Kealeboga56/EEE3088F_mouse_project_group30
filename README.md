# Micromouse Project: Sensing and Power Subsystems

This repository contains the design files, schematics, and other relevant resources for the sensing and power subsystems of the Micromouse project. The repository is organized into two main folders: `sensing` and `power`.

## Sensing Subsystem

The `sensing` folder contains all the files related to the design and implementation of the sensing subsystem, responsible for obstacle detection and navigation. It includes the following:

- `schematics/`: This directory contains the schematic files for the sensing circuit, including the main schematic and any supplementary schematics.
- `pcb/`: This directory houses the PCB design files, including the board layout, Gerber files, and any other relevant PCB design files.
- `firmware/`: This directory contains the firmware code for the microcontroller used in the sensing subsystem, along with any libraries or dependencies required.
- `simulations/`: This directory includes any simulation files or models used for testing and validating the sensing subsystem's performance.
- `datasheets/`: This directory contains datasheets for the components used in the sensing subsystem, such as sensors, microcontrollers, and other integrated circuits.
- `docs/`: This directory houses any additional documentation or reports related to the sensing subsystem, such as design specifications, test reports, or user manuals.

## Power Subsystem

The `power` folder contains all the files related to the design and implementation of the power subsystem, responsible for power management and distribution. It includes the following:

- `schematics/`: This directory contains the schematic files for the power circuit, including the main schematic and any supplementary schematics.
- `pcb/`: This directory houses the PCB design files for the power subsystem, including the board layout, Gerber files, and any other relevant PCB design files.
- `firmware/`: This directory contains the firmware code for the microcontroller used in the power subsystem (if applicable), along with any libraries or dependencies required.
- `simulations/`: This directory includes any simulation files or models used for testing and validating the power subsystem's performance.
- `datasheets/`: This directory contains datasheets for the components used in the power subsystem, such as regulators, batteries, and other power management components.
- `docs/`: This directory houses any additional documentation or reports related to the power subsystem, such as design specifications, test reports, or user manuals.

## Importing footprints
- For importing footprints in kicad. the easyeda2kicad script was used.
- `Installation/`: run : "pip install easyeda2kicad" on your terminal
- for more on how to get the lcsc_id and how to import visit website [https://pypi.org/project/easyeda2kicad/]

## Contributing

If you would like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch for your feature or bugfix
3. Commit your changes to the new branch
4. Push the branch to your forked repository
5. Submit a pull request to the main repository

Please ensure that your contributions adhere to the project's coding standards and guidelines.

## License

This project is licensed under the [MIT License](LICENSE).
