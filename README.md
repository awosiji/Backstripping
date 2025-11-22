# Backstripping

# 1D Airy Isostasy Backstripping Tool  
### Stanford EPS 251 - Sedimentary Basins  
**Developed by Victor Awosiji (Stanford University)**  
*Created for [EPS 251](https://explorecourses.stanford.edu/search?q=EPS+251%3a+Sedimentary+Basins&view=catalog&filter-coursestatus-Active=on&academicYear=20252026): Sedimentary Basins, taught by Prof. Stephan Graham*

---

## Overview

Backstripping is a foundational technique used to reconstruct the tectonic subsidence history of sedimentary basins by progressively removing the effects of sediment loading and compaction.

This repository provides an automated **Python backstripping tool** implemented in Jupyter Notebook form. It allows students, researchers, and basin analysts to input custom stratigraphic data and instantly compute:

- Decompacted sediment thicknesses  
- Progressive burial and basin geometry  
- Tectonic subsidence curves  
- Depth-to-basement evolution through time  

The tool follows **1D Airy isostasy backstripping**, consistent with the methodology presented in:

- Allen & Allen (2013) – *Basin Analysis*  
- Standard compaction relationships and example data from COST-B2 well
- Earlier excel tool developed by [Brian Romans (Virginia Tech)](https://geos.vt.edu/people/Everyone/Brian-Romans.html)

---

## Quick Demo

1. Enter stratigraphic units (ages, depths).  
2. Run all cells in `backstripping_tool.ipynb`.  
3. Inspect tectonic subsidence and depth-to-basement curves.

---

## Conceptual Workflow

```text
Input Stratigraphy (ages, depths)
          |
          v
   Decompact Units
          |
          v
  Remove Water + Sediment Loads
          |
          v
  Compute Tectonic Subsidence
          |
          v
  Build Depth-to-Basement Curve
          |
          v
      Plot Results vs Time
