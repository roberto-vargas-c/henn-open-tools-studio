


# Facade Panelization

_A Grasshopper tool for automated facade panel placement and analysis from closed Breps (building envelopes)_

## Overview

**Facade Panelization** is a Grasshopper definition for Rhino that automates the process of subdividing (panelizing) facade surfaces of a building. Users input a closed Brep representing the building mass; the tool then extracts relevant facade surfaces and generates a rational panel grid for fabrication, visualization, or further architectural analysis.

---

## What This Tool Does

- Accepts a closed Brep (building envelope) as input.
- Identifies and extracts facade surfaces (building faces) for processing.
- Subdivides these surfaces into regular (e.g., rectangular or custom) panels according to user parameters.
- Outputs geometry representing each individual panel.
- Can calculate panel areas, centroids, and other metrics for downstream tasks.
- Places panels into clear groups or organizes data for easy export.

---

## Inputs and Parameters

- **Closed Brep:**  
  The main input geometry representing the building mass whose facades will be panelized.

- **Facade Block:**  
  Choose between the different facade blocks from the catalogue

- **Panelization Parameters:**  
  - Number of panels in V directions (e.g., vertical subdivisions)
  - Panel size controls (width, spacing)


---

## Outputs

- **Panel Blocks:**  
  Facade blocks following the previous panel subdivision

- **Data Export:**  
  Easy to bake blocks.

---

## Workflow / Logic

1. **Reference a closed Brep** in Rhino (representing your full building envelope).
2. The tool **extracts facade surfaces** 
3. Each facade surface is **subdivided into a grid (V directions)**, creating a rational panelization.
4. Output geometry for each panel is generated for visualization and export.
5. **Bake or export** panels as required for further 3D modeling, or documentation.

---

## Dependencies

- **Required:** Rhino 8 with Grasshopper
- **Built-in components:** Utilizes standard Grasshopper components.
- **Optional plugins:**  
  - [GhPython](https://www.food4rhino.com/en/app/ghpython) (for custom scripting, if present)
  - [UiPlus or Human](https://www.food4rhino.com/en/app/uiplus) (if custom UI or advanced display is present)

---

## Example Usage

1. Open `facade_panelization.ghx` in Grasshopper.
2. Connect your building (closed Brep) to the input.
3. Set the desired panelization parameters (number of subdivisions or panel sizes).
4. Visualize panelized facade in Rhino’s viewport.
5. Bake results for further use in your model or presentation.

---

## Credits

Developed using Grasshopper for Rhino. Includes logic for geometric processing and annotation.

---

## License

Specify your license (MIT, proprietary, etc.).

---