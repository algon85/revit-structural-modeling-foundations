# Tutorial: Model a Simple Structural Bay

In this tutorial, you will model a standard 20' x 20' structural bay. This involves placing vertical supports, connecting them with horizontal framing, and topping the system with a structural floor.

## Learning Objectives
* Place **Structural Columns** using a grid intersection.
* Connect members using the **Beam** tool.
* Create a **Structural Floor** with a defined span direction.

---

## Prerequisites
* A project with two levels: **Level 1** and **Level 2** (12' 0" height difference).
* A grid system consisting of **Grids 1, 2** and **Grids A, B** spaced at 20' intervals.

---

## Step 1: Place Structural Columns "At Grids"
Instead of placing columns one by one, we will use Revit's automation to snap them to our grid intersections.

1. Open the **Level 1** Floor Plan.
2. Go to **Structure** tab > **Column**.
3. In the Properties Palette, ensure a structural steel or concrete column is selected.
4. On the Ribbon, select the **At Grids** tool.
5. Drag a selection box over all four grid intersections (A1, A2, B1, B2).
6. Click the **Finish (Green Checkmark)** on the ribbon.

> **Note:** Check your 3D view. If the columns are "under" Level 1, ensure your placement mode was set to **Height** up to Level 2.

---

## Step 2: Add Structural Framing (Beams)
Beams are "Level-hosted," meaning they will be placed on the level you are currently viewing.

1. Open the **Level 2** Floor Plan (we want the beams to support this floor).
2. Go to **Structure** tab > **Beam**.
3. Similar to columns, select the **On Grids** tool.
4. Select all four grids. Revit will automatically place beams between the columns.
5. Click the **Finish** button.

---

## Step 3: Create the Structural Floor
Now we will "skin" the bay with a structural slab.

1. Remaining in the **Level 2** Floor Plan, go to **Structure** tab > **Floor**.
2. Select the **Pick Supports** tool (this is better than 'Pick Lines' for framing).
3. Click the four beams you just created. Revit will lock the floor edge to the beam centerline.
4. **Span Direction:** Notice the icon with two parallel lines on one edge of your sketch. This indicates which way the structural deck "spans." If you need to change it, click **Span Direction** and select a different edge.
5. Click the **Green Checkmark**.

---

