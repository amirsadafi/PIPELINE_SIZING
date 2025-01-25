# Pipeline Sizing: Engineering Procedure

This repository contains a Python implementation of a pipeline sizing algorithm based on engineering principles. The script leverages fundamental fluid mechanics equations to determine the optimal pipe diameter and ensures compliance with velocity and pressure drop constraints.

## Features

- **Accurate Calculations**: Implements Continuity Equation, Reynolds Number, and Darcy-Weisbach equations.
- **Iterative Design**: Adjusts pipe diameter iteratively to meet design criteria.
- **Flexibility**: Suitable for various industries requiring pipeline design.

## Inputs

The user provides the following inputs:

- **Mass Flow Rate**: Fluid mass flow rate (kg/s).
- **Density**: Fluid density (kg/m^3).
- **Viscosity**: Fluid dynamic viscosity (Pa.s).
- **Pipe Length**: Length of the pipeline (m).
- **Maximum Allowable Pressure Drop**: Maximum pressure drop across the pipeline (Pa).
- **Maximum Allowable Velocity**: Maximum velocity of the fluid (m/s).

## Outputs

The script returns:

- Optimal pipe diameter (m).
- Fluid velocity (m/s).
- Reynolds number.
- Darcy-Weisbach friction factor.
- Pressure drop (Pa).

## Example Usage

```python
from pipeline_sizing import pipeline_sizing

# Example input parameters
result = pipeline_sizing(
    mass_flow_rate=2.0,  # kg/s
    density=1000.0,      # kg/m^3
    viscosity=0.001,     # Pa.s
    pipe_length=50.0,    # m
    max_pressure_drop=50000.0,  # Pa
    max_velocity=3.0     # m/s
)

# Display results
for key, value in result.items():
    print(f"{key}: {value}")
```

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/pipeline-sizing.git
   ```
2. Navigate to the directory:
   ```bash
   cd pipeline-sizing
   ```
3. Run the Python script:
   ```bash
   python pipeline_sizing.py
   ```

## Contributions

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.


