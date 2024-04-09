# Micro-Mouse Sensing Subsystem

## Table of Contents
1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
3. [Subsystem Design](#subsystem-design)
   - [Design Decisions](#design-decisions)
   - [Failure Management](#failure-management)
   - [Final Design](#final-design)
   - [System Integration and Interfacing](#system-integration-and-interfacing)
4. [Testing and Validation](#testing-and-validation)
   - [Acceptance Testing](#acceptance-testing)
   - [Test Results](#test-results)
5. [Project Management](#project-management)
   - [Repository Structure](#repository-structure)
   - [Version Control](#version-control)
6. [Conclusion](#conclusion)
7. [Future Improvements](#future-improvements)
8. [References](#references)

## Introduction
This repository contains the design and implementation of the Sensing Subsystem for the Micro-Mouse project, which is part of the EEE3088F course at the University of Cape Town. The Sensing Subsystem is responsible for detecting obstacles in the path of the micro-mouse robot, providing critical information to the central Processor subsystem to enable the robot to navigate through the maze effectively.

## Project Overview
The Micro-Mouse project is a comprehensive hardware design and development exercise, where students are tasked with designing and implementing various subsystems that make up the complete micro-mouse robot. The project is divided into four main modules: the Processor, Motherboard, Sensing, and Power subsystems.

This repository focuses on the design and implementation of the Sensing Subsystem, which is responsible for detecting obstacles in the robot's path. The subsystem must meet specific requirements and interface with the other modules to enable the micro-mouse to navigate the maze successfully.

## Subsystem Design

### Design Decisions
The design of the Sensing Subsystem involved several key decisions, including the choice of sensors, the sensor configuration, the processing unit, and the power management strategy. These decisions were made based on the project requirements, constraints, and trade-offs between performance, power consumption, and cost.

[Provide a detailed description of the key design decisions, including the rationale behind each decision and the alternatives considered.]

### Failure Management
To ensure the reliability and robustness of the Sensing Subsystem, the design includes several failure management strategies, such as:

1. Sensor Redundancy: Using multiple IR proximity sensors to provide redundancy in case of sensor failure.
2. Sensor Calibration: Implementing a calibration procedure to maintain accurate and consistent sensor readings over time.
3. Watchdog Timer: Incorporating a watchdog timer in the microcontroller to detect and recover from potential software or hardware faults.

[Describe each failure management strategy in more detail, explaining how it contributes to the overall reliability of the subsystem.]

### Final Design
The final design of the Sensing Subsystem includes the following key components:

- 3 IR proximity sensors (1 front-facing, 2 side-facing)
- STM32F051 microcontroller to manage the sensors and communicate with the Processor subsystem
- On/off switch for power-save mode

[Provide a detailed description of the final design, including schematics, PCB layouts, and any other relevant information. Explain how the design meets the project requirements and constraints.]

### System Integration and Interfacing
The Sensing Subsystem is designed to integrate seamlessly with the other modules of the Micro-Mouse project. The subsystem connects to the Motherboard through a 2x14 pin header, with specific pin assignments for sensor inputs, power, and communication with the Processor subsystem.

[Describe the pin-level interfacing between the Sensing Subsystem and the Motherboard, as well as the overall system-level integration, including a high-level block diagram.]

## Testing and Validation

### Acceptance Testing
The Sensing Subsystem has been subjected to a series of acceptance tests to verify its functionality and performance. These tests include:

1. Obstacle detection range test
2. Power consumption test
3. Processor interface test

[Provide details on each acceptance test, including the test procedure and the pass/fail criteria.]

### Test Results
The results of the acceptance testing have been recorded and analyzed. The Sensing Subsystem has successfully passed all the tests, demonstrating its ability to detect obstacles within the required ranges, maintain the specified power consumption levels, and communicate effectively with the Processor subsystem.

[Summarize the test results and discuss any issues or areas for improvement identified during the testing process.]

## Project Management

### Repository Structure
This repository is organized as follows:

```
micromouse-sensing/
├── docs/
│   ├── interim-design-report.pdf
│   └── final-report.pdf
├── hardware/
│   ├── schematic/
│   ├── pcb/
│   └── bom/
├── software/
│   ├── src/
│   └── include/
├── tests/
│   ├── obstacle-detection/
│   ├── power-consumption/
│   └── processor-interface/
├── README.md
└── .gitignore
```

The key directories and their contents are:

- `docs/`: Contains the Interim Design Report and the Final Report for the Sensing Subsystem.
- `hardware/`: Includes the schematic, PCB design files, and the Bill of Materials (BOM) for the Sensing Subsystem.
- `software/`: Contains the source code and header files for the software component of the Sensing Subsystem.
- `tests/`: Holds the test scripts and data for the acceptance testing of the Sensing Subsystem.

### Version Control
This project uses Git for version control. All changes to the design, software, and documentation are tracked using Git commits and branches. The main branch (`main`) is used for the final, approved version of the project, while feature branches are used for developing and testing new components or changes.

## Conclusion
The Sensing Subsystem design has been successfully implemented and tested, meeting all the project requirements and constraints. The subsystem's ability to reliably detect obstacles in the micro-mouse's path, while maintaining low power consumption, is a critical component in enabling the overall robot to navigate the maze efficiently.

## Future Improvements
While the current design of the Sensing Subsystem meets the project requirements, there are several areas where improvements could be made in the future:

1. Explore alternative sensor technologies: Investigate the use of other sensor types, such as ultrasonic or laser-based sensors, to potentially improve the detection range or accuracy.
2. Enhance power management: Optimize the power-save mode functionality to further reduce the subsystem's power consumption during periods of inactivity.
3. Improve sensor fusion: Investigate methods to combine the data from multiple sensors to provide a more robust and reliable obstacle detection capability.

## References
1. EEE3088F Project Brief, Department of Electrical Engineering, University of Cape Town, 2024.
2. STM32F051 Reference Manual, STMicroelectronics, 2019.
3. LV-MaxSonar-EZ1 Datasheet, MaxBotix Inc., 2013.
