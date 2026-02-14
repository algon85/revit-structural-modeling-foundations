# Tutorial: Creating a Structural Core

Building a structural core is a foundational task in Revit. In this tutorial, you will model a central shear wall system and host it on a structural slab. This exercise focuses on parametric constraints and the "Pick Lines" workflow.

## Learning Objectives
By the end of this tutorial, you will be able to:
* Set up structural wall constraints correctly.
* Use the **Pick Lines** tool to align walls to an existing grid.
* Generate a **Structural Foundation Slab** hosted by walls.

---

## Prerequisites
* A Revit project file with a basic Grid System (A-D, 1-4).
* Levels defined for **T.O. Foundation** and **Level 1**.
* The **Structural Wall** family loaded (typically "Basic Wall - Generic - 12\"").

---

## Step 1: Define Wall Constraints
Before placing geometry, we must define the vertical boundaries to ensure the model remains parametric.

1. Open the **Level 1** Floor Plan view.
2. Navigate to the **Structure** tab > **Structure** panel > **Wall: Structural**.
3. In the **Properties Palette**, configure the following:
   * **Base Constraint:** T.O. Foundation
   * **Top Constraint:** Level 1
   * **Structural Usage:** Shear
   * **Location Line:** Core Face: Interior



---

## Step 2: Model the Core Walls
We will use the grid lines as the "skeleton" for our walls to ensure they move if the building footprint changes.

1. On the **Modify | Place Structural Wall** tab, select the **Pick Lines** tool.
2. Hover over the grid lines defining your core (e.g., Grids B, C, 2, and 3).
3. Click to place the walls. 
   * *Tip: If the wall appears on the wrong side of the grid, press `Spacebar` to flip it.*
4. Use the **Trim/Extend to Corner (TR)** tool to join the wall corners into a closed loop.



---

## Step 3: Add the Foundation Slab
The core walls require a structural foundation to distribute the load.

1. Switch to the **T.O. Foundation** floor plan view.
2. Go to the **Structure** tab > **Foundation** panel > **Slab (Structural Foundation: Slab)**.
3. In the **Modify | Create Floor Boundary** tab, select the **Pick Walls** tool.
4. Select the four walls created in Step 2. 
5. In the Options Bar, ensure **Extend into wall (to core)** is checked. This ensures the slab edge aligns with the structural layer of the wall.
6. Click the **Green Checkmark** to finish the sketch.



---

## Result
You have successfully modeled a structural core that is constrained to both the project levels and the grid system. 

### Next Steps
* **How-To:** [How to Modify Structural Foundations](../how-to/how-to-modify-structural-foundations.md)
* **Explanation:** [Understanding Structural vs. Architectural Walls](../explanations/explanation-structural-vs-architectural-elements.md)
* **Reference:** [Structural Element Type Properties](../reference/reference-structural-element-types.md)   
