# Reference: Structural Element Behaviors & Placement

A quick-lookup guide for the placement logic and parametric behaviors of Revit structural elements.

---

## Placement Logic: Height vs. Depth
When placing vertical elements (Columns), the **Options Bar** determines the vertical direction.

| Element Type | Default Setting | Logic |
| :--- | :--- | :--- |
| **Architectural Column** | **Height** | Placed from the floor up. Used for aesthetics/cladding. |
| **Structural Column** | **Depth** | Placed from the top-down. Represents load-bearing support for the current level. |


> **Troubleshooting:** If a Structural Column is "invisible" upon placement, check if it was placed in **Depth** mode. It likely exists below your current View Range.

---

## Foundation Types
Revit categorizes foundations by how they "attach" to the rest of the building.

| Foundation Tool | Hosting Behavior | Typical Use Case |
| :--- | :--- | :--- |
| **Isolated** | Hosted by Columns | Spread footings, pier pads. |
| **Wall** | Hosted by Walls | Continuous strip footings. |
| **Slab** | Self-Hosted (Sketch) | Driveways, Patios, Mat foundations. |

---

## Essential Keyboard Shortcuts (Structure)
Speed is key in professional modeling. Use these to skip the Ribbon menu:

* **WA:** Wall (Note: Defaults to Architectural; use Structure tab for Structural Walls)
* **CL:** Structural Column
* **BM:** Structural Beam
* **FT:** Structural Foundation: Isolated
* **TR:** Trim/Extend to Corner (Critical for cleaning up wall junctions)
* **AL:** Align (Essential for locking slabs to walls)
* **more to be added**

---

## Discipline Visibility States
How the **View Discipline** property affects what you see:

* **Structural:** Prioritizes bearing elements. Non-structural walls appear transparent/halftone.
* **Architectural:** Shows finishes, furniture, and partitions. Structural Analytical lines are hidden.
* **Coordination:** Shows everything. Used for checking if pipes hit beams or if columns block doors.
