# Hardware Design Files

The KiCad material is organized by function because the supplied project history contains separate PCB layouts for the analog front-end and the ESP32/power section, while the final schematic combines the system blocks.

## Final system schematic

`kicad/schematic/SENS-CO_final_system.kicad_sch`

Contains the report-aligned system with the ESP32-S3-MINI-1, TPS78233 regulator, LIR2450 supply, LMP7721 transimpedance amplifier, LTC1044 voltage inverter, 100 MΩ feedback resistor, and sensor interface.

## PCB layouts

- `kicad/pcb/SENS-CO_analog_frontend.kicad_pcb` — routed analog front-end PCB including the LMP7721/LTC1044 section and high-impedance layout work.
- `kicad/pcb/SENS-CO_esp32_power.kicad_pcb` — ESP32-S3-MINI-1 and power-management PCB section.

## Custom symbols

`kicad/libraries/SENS-CO_custom_symbols.kicad_sym`

The original development folder also contained experimental/earlier alternatives (EFR32BG22, LM27761, TPS60400) and local KiCad backup/cache files. They are intentionally excluded from this recruiter-facing repository because they are not part of the final report architecture.
