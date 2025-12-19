Program Areas V_2
A Grasshopper tool for area computation and visualization of building massings

Overview
Program Areas V_2 is a Grasshopper script for Rhino that calculates and visualizes the areas of closed polysurfaces (building massings) in architectural studies. It computes the area and centroid for each mass and generates an easy-to-read area graph for use in analysis and presentations. The script supports grouping, color-coding, and annotation out-of-the-box.

What This Tool Does
Calculates the surface area of each input building mass (closed polysurface/Brep)
Finds the centroid of each mass for smart placement of labels
Groups and color-codes each mass for legibility in diagrams
Outputs area data both as text (labels and legends) and as grouped colored geometry in the viewport
Supports additional grouping, annotation, or panel customization
Inputs and Parameters
Closed Polysurfaces (Breps):
Represent individual buildings or zones. These must be closed volumes for correct area calculation.
[Optional] Names or IDs:
Assign to each Brep for better labeling.
[Optional] Custom Colors:
Pick colors for visual grouping of the masses.
[Optional] Site Boundary:
For context or area percentage calculations.
[Optional] Units:
Choose (e.g., SI or Imperial) for output display.
Outputs
Area per Mass:
Numeric value calculated for each mass (displayed as text).
Centroid for Labeling:
The centroid of each mass, used for label placement.
Visualization:
Each mass colored/grouped (for easy reading in viewport)
Area text appears at centroid or in a legend/panel
Summary Panel or Legend:
(Optional) overall statistics (e.g. total area, comparative areas, area percentages).
Geometry Export:
Colored masses, text, and panels can be baked for documentation or presentations.
Workflow / Logic
Reference or create closed polysurfaces for each building mass in Rhino.
(Optional) Assign IDs, colors, or groupings for clarity.
The script computes area and centroid for every mass using Grasshopper’s Area component.
Area values are displayed as labels at the centroid or in a summary panel.
Masses are grouped and color-coded for visual clarity and quick understanding of area breakdowns.
Results can be baked/exported for reports or presentation graphics.
Dependencies
Required: Rhinoceros 6/7/8 + Grasshopper
Plugins:
UiPlus (for interface/panels)
froGH (geometry/data tools)
CORE Toolbox (CORE studio utils)
Pufferfish (advanced geometry manipulation)
(If plugins are optional or mainly for UI/panels, the basic workflow remains supported natively)

Example Usage
Open Program Areas V_2.ghx in Grasshopper.
Set the input Breps (building masses).
Review area labels and color-coded geometries in the Rhino viewport.
Extract or bake results as needed for your workflow.
Credits
Developed using Grasshopper and selected add-ons by the parametric design community.

License
Specify your license here (MIT, proprietary, etc.).

Questions/Feedback?
Contact the script author or open an issue in the repository if available.