# Reference: Selection Sets and Model Groups

This reference guide outlines the differences, use cases, and management workflows for **Selection Sets** and **Model Groups** within a structural context.

---

## 1. Selection Sets
Selection Sets allow you to save a specific collection of elements so you can quickly re-select them later without manual filtering.

### Key Use Cases
* **Visibility Overrides:** Quickly hide or color-code all "Level 1 Shear Walls."
* **Scheduling:** Isolating a specific group of elements for a custom material takeoff.
* **Filter Rules:** Using a saved selection as the basis for a View Filter.

### Management Commands
* **Save:** After selecting elements, go to **Modify** tab > **Selection** panel > **Save**.
* **Load:** Go to **Manage** tab > **Selection** panel > **Load**.
* **Edit:** Add or remove elements from an existing set via the **Edit** button in the Selection panel.



---

## 2. Model Groups
Model Groups are collections of elements that represent a repeating unit of the building. When you edit one group, every other instance of that group in the project updates automatically.

### Key Use Cases
* **Standard Structural Bays:** Grouping the columns, beams, and slabs of a 20x20 bay to repeat across a grid.
* **Stair Towers:** Grouping structural walls and stairs for multi-story repetition.
* **Unit Layouts:** In residential structures, grouping the load-bearing interior partitions.

### Management Commands
* **GP:** Keyboard shortcut to create a group.
* **Edit Group:** Allows you to add/remove members or modify geometry within the group "container."
* **Ungroup:** Breaks the association, turning the items back into individual elements.



---

## Comparison: Which tool should you use?

| Feature | Selection Sets | Model Groups |
| :--- | :--- | :--- |
| **Purpose** | Workflow efficiency & Filter logic. | Geometric repetition & Consistency. |
| **Geometry** | Elements remain independent. | Elements are "locked" into a unit. |
| **Changes** | Changing one element only affects that one. | Changing one group instance updates all. |
| **Visibility** | Used to trigger View Filters. | Can be excluded or hidden as a unit. |

---

## Best Practices for Structural Modeling

### The "Don't Over-Group" Rule
Avoid grouping elements that are hosted by different levels (e.g., don't group a Level 1 column with a Level 2 beam). This often causes "Group Instance" errors. Keep groups restricted to a single floor whenever possible.

### Selection Sets for QC
Create a Selection Set called "Structural-Analytical-Review." Use it to quickly grab all primary load-bearing members to verify their analytical nodes are aligned before exporting to analysis software.

### Naming Conventions
* **Sets:** `SEL_Floor-01_Shear-Walls`
* **Groups:** `GRP_20x20-Steel-Bay`
