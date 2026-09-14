# Title-24-Complex-HVAC-Energy-Models
Public repository of downloadable CBECC model files supporting the **CBECC Complex HVAC Example Guide**, organized by example.

## About This Project
California's performance pathway gives buildings real flexibility. A design team can trade energy across systems, take credit for what the building does, and find compliance in a form that fits the project instead of a prescriptive checklist. That flexibility only pays off if the model is right. The modeler has to build it correctly, the design team needs to understand what was assumed on their behalf, and the finished building has to match what the model claimed.

Mechanical systems are where that breaks down first. They are the hardest thing compliance software asks a modeler to represent, and the least forgiving when the representation is wrong.

This repository holds working CBECC model files for eight complex HVAC configurations that come up frequently in Title 24 projects and are often modeled incorrectly, along with seven alternates that show how the model changes when the system architecture does. Each example is paired with documentation that runs from the mechanical system as designed, through the CBECC object hierarchy, to the specific inputs used. Models are supplied pre-simulated, with their results and compliance files included.

Full guidance documentation and system diagrams are hosted on the CalBEM website: **https://calbem.ibpsa.us/cbecc-complex-hvac-project/**

## Attribution
Developed by A2 Efficiency with support from Southern California Edison (SCE) and the California IOUs under CalBEM Working Group 3.

## Model and Software Version
For the initial release batch:
- **Version:** `v1.0`
- **CBECC version used:** `CBECC 2025.2.0.1 (1395)`

## Folder Structure
Each `Example-Guide.pdf` is that example's PDF write-up (actual filenames are per example, e.g. `Example 1 - MF Ventilation Options and Split Heat Pumps.pdf`). Examples 1, 5, and 8 group design variants under `v1.0/` (`1a`–`1e`, `5a`/`5b`, `8a`/`8b`); the others keep their model files directly in `v1.0/`.

```text
Models/
  EX01_MF_Ventilation/
    Example-Guide.pdf
    v1.0/
      1a/  1b/  1c/  1d/  1e/        # each variant holds the CBECC model folder(s)
  EX02_MF_Central-VRF-HP/
    Example-Guide.pdf
    v1.0/                            # model files
  EX03_MF_Central-WSHP/
    Example-Guide.pdf
    v1.0/                            # model files
  EX04_NR_SmOff_SZ-VAV-DF-HP/
    Example-Guide.pdf
    v1.0/                            # model files
  EX05_NR_SmOff_DOAS-VRF/
    Example-Guide.pdf
    v1.0/
      5a/  5b/
  EX06_NR_Class-Lab-DOAS-FPFC/
    Example-Guide.pdf
    v1.0/                            # model files
  EX07_NR_PVAV_PFPB/
    Example-Guide.pdf
    v1.0/                            # model files
  EX08_NR_Rstnt/
    Example-Guide.pdf
    v1.0/
      8a/  8b/
  index.csv
```

## Download Instructions
1. Browse to `Models/`
2. Open the desired example folder (e.g., `EX02_MF_Central-VRF-HP`); it contains the example PDF and a `v1.0/` folder
3. Open `v1.0/` (for Examples 1, 5, and 8, then open the variant subfolder, e.g., `1a/`)
4. Download the model files directly

Or clone everything:
```bash
git clone https://github.com/A2Efficiency/Title-24-Complex-HVAC-Energy-Models.git
cd Title-24-Complex-HVAC-Energy-Models
```

## Versioning Policy
- Version format: `vMAJOR.MINOR`
- MAJOR: changes that affect structure or compatibility
- MINOR: corrections or incremental updates
- Historical versions remain available for traceability
- CBECC version used for each release is documented here and in `Models/index.csv`, not in the folder path

## External Documentation
All technical documentation and specifications are maintained at:
**https://calbem.ibpsa.us/cbecc-complex-hvac-project/**

## License
Creative Commons Attribution 4.0 International (CC BY 4.0).
See [LICENSE](./LICENSE).

### Quick Guide for Modifying & Sharing:
* **Derivative Works:** You are entirely free to modify these CBECC models and license your new derivative variations under any terms you choose (including commercial or closed-source licenses).
* **Modifications Notice:** If you distribute or publish modified versions of these files, the CC BY 4.0 license legally requires you to state clearly that your files have been altered from our original baseline configurations.
* **Attribution:** Any public sharing or adaptation of this material must include credit to the original creators listed in the Attribution section above.

## Contributions & Issues
This repository does not accept pull requests. Please open an issue for missing or corrupt files, or naming and version errors:
`https://github.com/A2Efficiency/Title-24-Complex-HVAC-Energy-Models/issues`
