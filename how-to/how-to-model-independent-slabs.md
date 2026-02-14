# How-To: Create an Independent Structural Slab (Driveway)

This guide demonstrates how to create a "self-hosted" structural slab. This method is used for elements like driveways, patios, or equipment pads that exist independently of vertical structural elements like walls or columns.

## Overview

Unlike foundations hosted by walls, a driveway is defined by its own boundary sketch and is hosted directly to a **Level** or a **Reference Plane**.

---

## Instructions

### 1. Initialize the Slab Tool
1. Open the **Level 1** (or Grade) Floor Plan view.
2. Navigate to the **Structure** tab > **Foundation** panel.
3. Select **Slab (Structural Foundation: Slab)**.

### 2. Sketch the Boundary
Instead of using the "Pick Walls" tool, use the geometric draw tools to define a custom shape.
1. In the **Modify | Create Floor Boundary** tab, select the **Line** or **Rectangle** tool.
2. Sketch the perimeter of your driveway. 
3. **Tip:** Use the **Fillet Arc** tool if you need to create curved "flares" where the driveway meets the street.
4. Ensure the sketch forms a **closed loop** with no overlapping lines.

### 3. Set Offsets and Slope
Driveways often sit slightly below the finished floor level of a garage or house to prevent water ingress.
1. In the **Properties Palette**, locate **Height Offset from Level**.
2. Set this to a negative value (e.g., `-0' 2"`) to account for a threshold.
3. **Optional (Drainage):** Select the **Slope Arrow** tool and draw it from the garage toward the street. In the Properties Palette, define the "Slope" percentage (e.g., 2%) to ensure water runoff.

### 4. Finish the Element
1. Click the **Green Checkmark** to finish the sketch.

---

## Key Differences from Hosted Slabs
* **Manual Control:** If the building moves, the driveway will stay in its original coordinates unless you manually move it or use the **Align (AL)** tool to lock the sketch lines to the building's footprint.
* **Hosting:** This slab is hosted by the **Level**, meaning it responds to changes in the project's vertical datum (the height of the level) rather than the movement of walls.

---

## Related Documentation
* **Tutorial:** [Creating a Structural Core](../tutorials/tutorial-create-structural-core.md)
* **Explanation:** [Hosted vs. Self-Hosted Elements](../explanations/explanation-material-association-and-behavior.md)
