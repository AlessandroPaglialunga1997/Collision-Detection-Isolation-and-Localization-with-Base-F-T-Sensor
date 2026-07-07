# Collision Detection, Isolation, and Localization with Base Force/Torque (F/T) Sensor

## Overview
This repository contains a Simulink model and supporting materials for detecting, isolating, and localizing collisions using a base-mounted force/torque (F/T) sensor. The primary artifact is the Simulink model that acquires F/T data, detects collision events, isolates the source, and estimates the collision location.

## Requirements
- MATLAB with Simulink (recommended: R2018b or later)
- Hardware support package or driver for the F/T sensor if using real hardware
- Optional: additional MATLAB toolboxes for visualization or data logging depending on your configuration

## Project Structure
- [Main.slx](Main.slx) — main Simulink model
- README.md — this file
- `Detailed_Report.pdf` (or `Detailed_Report.md`) — a comprehensive report that documents the manipulator used for the simulation, the Simulink blocks and subsystems used to perform the three required tasks (Detection, Isolation, Identification), and the results of the experiments.
- `Presentation.pptx` — a PowerPoint presentation summarizing the approach, experiments, and key results.

## Reports and Presentation
The repository includes a detailed report and a presentation:

- The detailed report describes:
	- the manipulator model used for the simulation (kinematics, link parameters),
	- the Simulink blocks/subsystems used to implement each of the three tasks (Detection, Isolation, Identification),
	- parameter settings and configuration details required to reproduce the experiments,
	- experimental results, plots and analysis.

- The PowerPoint presentation provides a concise overview of the methodology, experiment setup, and summarized results suitable for demonstrations or oral presentations.

## Getting Started
1. Open MATLAB and set the project folder as the current working directory or add it to the MATLAB path.
2. Open the Simulink model: open [Main.slx](Main.slx).
3. Inspect model parameters (sample rate, sensor channel names, logger settings) and adapt them to your setup.
4. If using physical hardware, configure the sensor interface and drivers according to the vendor instructions.
5. Run the simulation or real-time model using the Simulink `Run` button. Monitor outputs via Scopes, Dashboard blocks, or logged files.

## Key Parameters
- Sensor sampling frequency
- Detection thresholds for collision/event detection
- Filter and denoising parameters

## Expected Outputs
- Collision detection flags/events (boolean)
- Estimated collision location (link/joint or Cartesian coordinates)
- Logged data for post-processing and analysis

## Authors
- Author: (Add your name and contact information)

## License
No license specified. Add a `LICENSE` file to the project root to apply a license (e.g., MIT, Apache-2.0).

## Contributing
Feel free to open issues or submit pull requests to report bugs, request features, or propose improvements.

