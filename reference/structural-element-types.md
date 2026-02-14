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
