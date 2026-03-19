# System Identification of 10-DOF VTOL Drone 📊

This module focuses on developing a data-driven model of the VTOL drone using system identification techniques. The goal is to approximate the system dynamics using input-output data instead of relying purely on physics-based modeling.

## Current Functionality:

* Input-output data collected from simulation
* Data preprocessing (filtering and trimming)
* Model estimation using N4SID (Subspace Identification)
* Order sweep performed to determine optimal system order
* Model validation using fit percentage and residual analysis

## Methodology:

1. Generate input-output data from simulation
2. Preprocess data (remove noise, trim signals)
3. Apply N4SID algorithm
4. Sweep model order (1–16)
5. Select best model based on:
   - Minimum RSS (Residual Sum of Squares)
   - Maximum fit percentage

## Sample Result:

![System ID](Simscape_Model/Screenshots/system_id.png)

## Files:

* `system_id.m`
* `data.csv`
* `identified_model.mat`

## Output:

* State-space model of the VTOL system
* Fit comparison plots
* Residual analysis

## Future Work:

* Improve model accuracy with better excitation signals
* Include nonlinear identification techniques
* Real-time system identification
