# attack_scenarios

Attack scenario generators for stress testing the Ψ-Risk-DT framework.

## Structure
- `scenario_config.yaml` - run configuration
- `scenario_generator/` - attack modules
  - `udp_flood.py` - UDP volumetric flood attack pattern for high packet rate stress testing
  - `entropy_anomaly.py` - zero-day like attack with unusual entropy characteristics
  - `escalation_attack.py` - structured attack divided in 3 distinct phases (Stealth, Ramp-up, Saturation)

## Usage
1. Install the requirement
1. Adjust `scenario_config.yaml` if necessary.
2. Run the desired module (e.g. `python scenario_generator/udp_flood.py`).
