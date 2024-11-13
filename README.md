# ISD_ReuseConcrete
<br/> Resource for students inStÖk, CaDP Seminar at i.sd, University of Innsbruck
<br/> created by Muchen Yan
<br/> Code used in the Grasshopper scripts referenced open-source solutions  
To work with the files in this repository, please ensure the following software and plugins are installed:

- **Rhinoceros 7 or 8** – for 3D modeling and integration with Grasshopper.
- **Grasshopper Plugins**:
  
  - **OpenNest** – for arranging and nesting elements within the design.
  - **Pufferfish** –
 
Import from Rhino to Blender for rigid body simulation:
 - Export from Rhino as obj.
 - Import obj. in Blender, change the scale to 0.001 in the import options
 - click on the imported(the objects are in one group), change to Edit Mode, press P, select "By Loose Parts"
 - Now each objects are separated. Select all of them, press Control + A, select scale. The scale transformation should be reset to 1 after this.
 - Select all the obejects, go to object - Set Origin - Origin to Geometry. A little orange point should be in the centre of each object after this.
 - Select one of the obejct, add rigid body. Then object - rigid body - calculate mass - concrete.
 - adjust parameters in rigid body setting.
 - Select all other objects first and the edited object last, go to object - rigid body - copy from active.
 - calculate mass for each piece.
<br/> **Ackonwledgement:** Code used in the Grasshopper scripts referenced open-source solutions. Including: <br/> https://github.com/dantaeyoung/GrasshopperArsenal/tree/master/HungarianAlgorithm <br/> https://github.com/bonalan/From-Waste-to-Resource/tree/main
