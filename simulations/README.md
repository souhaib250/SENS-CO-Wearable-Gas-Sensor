# Analog Front-End Simulations

This directory contains the simulation results used to study the high-impedance analog front-end described in the project report.

Two precision amplifiers were evaluated:

- ADA4530-1
- LMP7721

The comparison includes transient response, output voltage versus sensor resistance, and output voltage versus sensor conductance.

The final hardware design uses the LMP7721 with a 100 MΩ feedback resistor. The sensor is represented by a resistance in the hundreds-of-megaohms range.

## Results

### Transient response

| ADA4530-1 | LMP7721 |
|---|---|
| ![ADA4530-1 transient](results/transient/ADA4530-1_transient.png) | ![LMP7721 transient](results/transient/LMP7721_transient.png) |

### Sensor resistance sweep

| ADA4530-1 | LMP7721 |
|---|---|
| ![ADA4530-1 resistance sweep](results/resistance-sweep/ADA4530-1_resistance-sweep.png) | ![LMP7721 resistance sweep](results/resistance-sweep/LMP7721_resistance-sweep.png) |

### Sensor conductance sweep

| ADA4530-1 | LMP7721 |
|---|---|
| ![ADA4530-1 conductance sweep](results/conductance-sweep/ADA4530-1_conductance-sweep.png) | ![LMP7721 conductance sweep](results/conductance-sweep/LMP7721_conductance-sweep.png) |

## Reproducibility note

`data/LMP7721_resistance_sweep.csv` contains the exported DC sweep values and `data/LMP7721_resistance_sweep.wbk` contains the KiCad simulator workbook settings that were provided with the project files.

Vendor SPICE model files are not redistributed in this public-repository package because their redistribution terms were not established from the supplied files.
