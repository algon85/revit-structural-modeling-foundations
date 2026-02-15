# How-To: Assign and Edit Materials

This guide demonstrates the process of assigning materials to structural elements and modifying their graphic and physical properties.

## Overview
In Revit, materials are assigned either by **Category**, by **Element Type**, or by **Instance**. For structural modeling, the most common and "BIM-compliant" method is through **Type Properties**.

---

## Instructions

### 1. Accessing Material Properties
1. Select a structural element in your model (e.g., a Concrete Column or Steel Beam).
2. In the **Properties Palette**, click **Edit Type**.
3. Locate the **Materials and Finishes** section.
4. Click the small **[...] button** in the value field for "Structural Material." This opens the **Material Browser**.

### 2. Creating a New Material
Instead of overwriting default materials, it is best practice to create a duplicate.
1. In the Material Browser, right-click an existing material (e.g., "Concrete, Cast-in-Place").
2. Select **Duplicate with Assets**.
3. Rename it (e.g., "ST-Concrete - 4000 PSI").

### 3. Editing Material Graphics
This determines how the material looks in your documentation.
1. **Surface Pattern:** Set the pattern used in 3D or Elevation views (e.g., "Sand" for concrete).
2. **Cut Pattern:** Set the pattern used in Section or Floor Plan views (e.g., "Concrete" hatch). 
3. **Color:** Change the shading color for "Shaded" or "Consistent Colors" visual styles.

### 4. Reviewing Physical Assets
For structural modeling, the **Physical** tab is the most critical.
1. Click the **Physical** tab in the Material Browser.
2. Ensure the **Mechanical** properties (Young's Modulus, Poisson's Ratio) match your project's engineering specifications.
3. These values are what Revit exports to structural analysis software.

---

## Best Practices

---

## Related Documentation
* **Explanation:** [Material Association and Behavior](../explanations/explanation-material-association-and-behavior.md)
* **Reference:** [Structural Element Types](../reference/reference-structural-element-types.md)
