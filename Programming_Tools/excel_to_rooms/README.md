

---

# Excel to rooms

_A Grasshopper tool for generating room/area data from Excel for architectural workflows_

## Overview

**excel_to_rooms.ghx** is a Grasshopper definition designed to streamline the translation of room or area data from Excel spreadsheets directly into Rhino/Grasshopper for architectural analysis and visualization. It reads structured Excel data, processes room/area parameters, and generates geometric and annotation outputs, enabling fast spatial programming and schematic diagramming.

---

## What This Tool Does

- Reads room/area data (names, dimensions, parameters) from an Excel spreadsheet.
- Generates corresponding geometry (e.g., boxes representing each room).
- Calculates and displays areas for each room.
- Places 3D text tags in the viewport to annotate rooms with names, area values, or other data.
- Organizes rooms into color-coded groups for easy visual review.
- Supports updating geometry quickly from new or edited Excel files with the push of a button.

---

## Inputs and Parameters

- **Excel Spreadsheet:**  
  Must contain a list of rooms/areas with at least:
  - Room Names
  - Room Types
  - Dimensions (length/width, or area)
  - Number of rooms

- **File Path:**  
  Set or select the source Excel file.

- **Column Mapping:**  
  Select excel columns according to the categories

- **Room Graph:**  
  Visualization options.



---

## Outputs

- **Room Geometry:**  
  Generated geometry for each room (e.g., rectangle Brep or other shapes as required).


- **Grouped Visualization:**  
  Rooms grouped by function, color, or any Excel-supplied data.


- **Updatable Results:**  
  Geometry and labels update when Excel is changed and the refresh button is pressed.

---

## Workflow / Logic

1. **Prepare your Excel spreadsheet** with room data (names, sizes, optional group/type info).
2. **Point to the Excel file** in the Grasshopper definition.
3. The script **reads the data, builds geometry** for each room based on input parameters.
4. Geometry and labels can be **baked into Rhino** for later drawing or documentation.

---

## Dependencies

- **Rhino 8 + Grasshopper**
- **Excel read plugin required**  
  _(Commonly used: [LunchBox](https://www.food4rhino.com/en/app/lunchbox), [Bumblebee](https://www.food4rhino.com/en/app/bumblebee), or similar)_

- **Optional:**  
  - [Heteroptera](https://www.food4rhino.com/en/app/heteroptera) (geometry/data utilities)

---

## Example Usage

1. Save your Excel file in a known location with proper structure.
2. Set the file path in the script as required.
3. Add or edit room data in Excel and refresh in Grasshopper.
4. Check that rooms, areas, and labels appear and are correct.
5. Export, bake, or annotate as needed.

---

## Credits

Script and logic by the parametric design community and/or your office/author name here.

---

## License

Specify license here (e.g., MIT, proprietary).

---

**Questions/Feedback?**  
Contact the author or open an issue in this repository.