# Volume Areas

_A Grasshopper tool for area computation and visualization of building massings_

## Overview

**Program Areas V_2** is a Grasshopper script for Rhino that calculates and visualizes the areas of closed polysurfaces (building massings) in architectural studies. It computes the area each mass and generates an easy-to-read area graph for use in analysis and presentations. The script supports grouping, color-coding, and annotation out-of-the-box.

---

## What This Tool Does

- Calculates the surface area of each input building mass (closed polysurface/Brep)
- Groups and color-codes each mass for legibility in diagrams based on its layer
- Outputs area data both as text (labels and legends)
- Supports additional grouping, annotation, or panel customization

---

## Inputs and Parameters

- **Closed Polysurfaces (Breps):**  
  Represent individual buildings or zones. These must be closed volumes for correct area calculation.

- **Layers:**  
  Assign to each Brep for better labeling.

- **Custom Colors:**  
  Pick colors for visual grouping of the masses.

- **Site Boundary Areas:**  
  For context or area percentage calculations.



---

## Outputs

- **Area per Mass:**  
  Numeric value calculated for each mass (displayed as text).


- **Visualization:**  
  - Each mass colored/grouped (for easy reading in viewport)
  - Area text appears in a legend/panel

- **Summary Panel or Legend:**  
  (Optional) overall statistics (e.g. total area, comparative areas, area percentages).

- **Graph Export:**  
  Colored graph can be baked for documentation or presentations.

---

## Workflow / Logic

1. **Reference or create closed polysurfaces** for each building mass in Rhino.
2. Assign **layers** and consecuent colors, or groupings for clarity.
3. The script computes **area** for every mass using Grasshopper’s Area component.
4. **Area values** are displayed as labels in a summary panel.
5. **Results can be exported** for reports or presentation graphics.

---

## Dependencies

- **Required:** Rhinoceros 8 + Grasshopper
- **Plugins:**
  - [UiPlus](https://www.food4rhino.com/en/app/uiplus) (for interface/panels)
  - [froGH](https://www.food4rhino.com/en/app/frogh) (geometry/data tools)
  - [CORE Toolbox](https://core.thorntontomasetti.com/tools/toolbox/) (CORE studio utils)
  - [Pufferfish](https://www.food4rhino.com/en/app/pufferfish) (advanced geometry manipulation)



---

## Example Usage

1. Open `volume_areas.gh` in Grasshopper.
2. Set the input Breps (building masses).
3. Review area labels and color-coded geometries in the UI Plus viewport.
4. Export results as needed for your workflow.

---

## Credits

Developed using Grasshopper and selected add-ons by the parametric design community.

---

## License

Specify your license here (MIT, proprietary, etc.).

---

**Questions/Feedback?**  
Contact the script author or open an issue in the repository if available.

---
