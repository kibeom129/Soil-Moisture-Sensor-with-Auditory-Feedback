## Project Demonstration Video

Click on the image below to watch the project demonstration video:

[![Watch the video](https://drive.google.com/uc?export=view&id=1QTKWaGymuPY3Xzg6ghPv-Yo3G9B-tt9C)](https://drive.google.com/file/d/1QTKWaGymuPY3Xzg6ghPv-Yo3G9B-tt9C/view?resourcekey)

## Project Presentation Slides

For a detailed overview of our project, including diagrams, technical details, and our development process, view our presentation slides:

[View Presentation Slides](https://docs.google.com/presentation/d/1W93WGzWNciMMUmCuppMuS06Y-gGXBqqM1IL80uMkibQ/edit#slide=id.p3)

## Introduction

In this final project for our EE14 Embedded Systems course, we, Senri Nakamura and Brian Kim, aim to innovate traditional soil moisture detection by developing a system that utilizes a TL555 timer-based circuit interfaced with the STM32L4 Cortex-M4 microcontroller. This system is designed to monitor soil moisture levels accurately, providing essential information for applications in agriculture, gardening, and environmental monitoring. Our unique approach incorporates auditory feedback to convey soil moisture status, facilitating use in various lighting conditions, including complete darkness.

## Background and Functionality

Effective moisture management is crucial for the vitality of crops and the sustainability of environmental ecosystems. While existing solutions typically rely on visual or digital displays, our project seeks to convey soil moisture levels through auditory feedback. This method aims to enhance usability for individuals with visual impairments and in scenarios where visual monitoring is impractical. Moreover, this sensor could be implemented in automated vertical farming.

Leveraging the TL555 timer's versatility, we plan to simulate soil moisture conditions, translating them into auditory signals generated by the STM32L4 microcontroller. This application of the TL555 timer allows for a robust, corrosion-resistant system capable of providing immediate and intuitive feedback about soil conditions through changes in sound frequency, pitch, or volume.

## Technical Approach/Framework

### Core Components

- STM32L4 Cortex-M4 Microcontroller
- TL555 Timer Circuit
- Speaker for auditory feedback (CL0201MA)

### Functionality

1. **TL555 Timer Circuit Simulation**: The TL555 is configured to simulate variable soil moisture conditions by generating frequencies or pulse widths that mimic the analog output you'd expect from a traditional soil moisture sensor.
2. **STM32L4 Interface**: The microcontroller reads the TL555's output, interpreting these signals to determine simulated moisture levels.
3. **Auditory Feedback**: Based on this interpretation, the STM32L4 activates the speaker to emit sounds that correspond to the detected moisture level, with unique tones indicating dry, moist, or wet soil conditions.

### System Diagram

*Include a visual diagram here showing the connections between the TL555 timer, STM32L4 microcontroller, and the speaker.*

## Tasks and Subtasks

### Hardware Setup

- Integrate the TL555 timer circuit with the STM32L4, ensuring accurate signal generation that corresponds to varying moisture levels.

### Software Development

- Program the STM32L4 to interpret the TL555 signals.
- Develop an algorithm for mapping these signals to moisture conditions.
- Implement logic for generating auditory feedback reflective of the moisture level.

### Testing and Calibration

- Test the TL555 circuit's output range and its correlation to simulated moisture conditions.
- Calibrate the auditory feedback system to ensure intuitive user interpretation.

### Documentation

- Document the system's design and implementation process.
- Prepare a user manual detailing the auditory feedback cues and their meanings.

## Evaluation Criteria

- **Accuracy**: Precision in simulating and interpreting soil moisture levels through the TL555 circuit.
- **Innovation**: Creative application of the TL555 timer for soil moisture simulation and the use of sound for feedback.
- **Technical Execution**: Effectiveness of the TL555 integration and the clarity of auditory signals produced.
- **User Accessibility**: Ease of understanding the auditory feedback and its correlation to soil moisture levels.

## Timeline (April 1st - April 26th)

- **Week 1**: Component procurement, initial setup, and TL555 integration with the STM32L4.
- **Week 2**: Firmware development for interpreting TL555 signals.
- **Week 3**: Auditory feedback refinement and system calibration.
- **Week 4**: Comprehensive system testing, documentation, and project presentation preparation.

## Individual Responsibilities

### Senri Nakamura: TL555 Integration, Signal Generation, and Data Processing

- **TL555 Timer Configuration**: Design and implement the circuit using the TL555 timer to simulate varying soil moisture levels.
- **Interface Design**: Develop the interface between the TL555 output and the STM32L4 microcontroller.
- **Signal Processing Software**: Write the firmware for the STM32L4 to process the input signals from the TL555.
- **Integration Testing**: Conduct initial tests to ensure the TL555 and STM32L4 are properly integrated.

### Brian Kim: Auditory Feedback Development, System Testing, and Documentation

- **Auditory Feedback System Design**: Design the auditory feedback mechanism that translates simulated soil moisture levels into audible signals.
- **PWM Control for Speaker**: Utilize the STM32L4's PWM outputs to drive the speaker.
- **System Testing and Calibration**: Lead comprehensive testing of the entire system to ensure accurate simulation of soil moisture levels and clear, understandable auditory feedback.

## Additional Resources

- [TLC555 Datasheet](https://pdf1.alldatasheet.com/datasheet-pdf/view/28905/TI/TLC555.html)
