New calculator and calibration workflow are now available

## Belter Calculator & Documentation Update

We’ve made a major update to the **BIQU Belter calculation workflow, Web Tool, and documentation** based on community feedback and additional testing.

### What’s New

- **Updated tension calculation model**
  - The calculator now uses the nonlinear model:
    `Tension = A / (dmax - d)^p`
  - Default parameters have been updated 


- **Custom calculation model calibration**
  - Advanced users can now generate their own **Coefficient A** and **Exponent p** from real test data.
  - The Web Tool supports test loads from **500 g to 2000 g in 100 g increments**.
  - The fitted model automatically reports **R²** and **RMSE** for reference.

- **Calibration data spreadsheet**
  - A new spreadsheet is provided for recording repeated measurements.
  - Each load can be measured **12 times**.
  - The highest and lowest readings are automatically removed.
  - The remaining 10 readings are used to calculate **Average (trimmed 10)** and **StDev**.

- **Direct Excel → Web Tool data import**
  - Copy the complete **Average (trimmed 10)** row from the calibration spreadsheet.
  - Paste it into any field under **Fit Parameters from Test Data**.
  - The Web Tool automatically maps the values from **500 g → 2000 g** and runs the model fit.

- **Custom Tension Range**
  - The previous **Belt Width** setting has been updated to **Tension Range**.
  - Existing presets remain unchanged:
    - GT2 6 mm
    - GT2 9 mm
  - A new **Custom Range** option allows users to define their own **Min / Max tension** values.

- **English / Chinese language support**
  - The Web Tool can now be switched directly between **English and Chinese**.

- **Updated calibration workflow**
  - Normal Belter calibration remains simple.
  - Custom calculation model calibration is an **optional advanced step**.
  - Users who do not need a custom model can continue using the default calculation parameters.

### Recommended Workflow

`Calibrate Belter → [Optional] Calibrate Calculation Model → Measure Belts Normally`

The goal of this update is to make the Belter workflow more transparent, repeatable, and flexible while keeping normal day-to-day measurements simple.

Special thanks to **@rongith** for providing experimental measurement data and to **@anokfireball** for contributing to the nonlinear tension model and technical discussion.

We’ll continue improving the Belter workflow based on real-world testing and community feedback.
