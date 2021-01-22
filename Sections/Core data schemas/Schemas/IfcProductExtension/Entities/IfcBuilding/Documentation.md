A building represents a structure that provides shelter for its occupants or contents and stands in one place. The building is also used to provide a basic element within the spatial structure hierarchy for the components of a building project (together with site, storey, and space).  
NOTE Definition from ISO 6707-1:    
Construction work that has the provision of shelter for its occupants or contents as one of its main purpose and is normally designed to stand permanently in one place.  
A building is (if specified) associated to a site. A building may span over several connected or disconnected buildings. Therefore building complex provides for a collection of buildings included in a site. A building can also be decomposed in (vertical) parts, where each part defines a building section. This is defined by the composition type attribute of the supertype _IfcSpatialStructureElements_ which is interpreted as follow:  
* **COMPLEX**: building complex
* **ELEMENT**: building
* **PARTIAL**: building section

  
  
The [<font color="#0000ff"><u>IfcBuilding</u></font>]($element://{6A41B6BC-5685-455c-84F7-0CBCEAF26389}) is used to build the spatial structure of a building (that serves as the primary project breakdown and is required to be hierarchical). The spatial structure elements are linked together by using the objectified relationship [<font color="#0000ff"><u>IfcRelAggregates</u></font>]($element://{12F56CBC-A6CE-493c-8A50-E301CE73BBA5}). Figure 150 shows the [<font color="#0000ff"><u>IfcBuilding</u></font>]($element://{6A41B6BC-5685-455c-84F7-0CBCEAF26389}) as part of the spatial structure. It also serves as the spatial container for building and other elements.  
NOTE Detailed requirements on mandatory element containment and placement structure relationships are given in view definitions and implementer agreements.  
  
[<font color="#0000ff"><u>Building composition</u></font>]($imageman://id=2006805526;mdg=Global;name=Building composition;type=Bitmap;)  
Figure 150 � Building composition  
  
Systems, such as building service or electrical distribution systems, zonal systems, or structural analysis systems, relate to [<font color="#0000ff"><u>IfcBuilding</u></font>]($element://{6A41B6BC-5685-455c-84F7-0CBCEAF26389}) by using the objectified relationship [<font color="#ff0000"><u>IfcRelReferencedInSpatialStructure</u></font>]($element://{415054A4-1479-4c32-9A58-BC1E36A488CC})<font color="#ff0000">.</font>  
Figure 151 describes the heights and elevations of the [<font color="#0000ff"><u>IfcBuilding</u></font>]($element://{6A41B6BC-5685-455c-84F7-0CBCEAF26389}) . It is used to provide the height above sea level of the project height datum for this building, that is, the internal height 0.00. The height 0.00 is often used as a building internal reference height and equal to the floor finish level of the ground floor.  
* base elevation of building provided by: _IfcBuilding.ElevationOfRefHeight_, it is usually the top of construction slab.
* base elevation of terrain at the perimeter of the building provided by: _IfcBuilding.ElevationOfTerrain_, it is usually the minimum elevation is sloped terrain
* total height of building, also referred to as ridge height (top of roof structure, e.g the ridge against terrain): provided by BaseQuantity with Name="TotalHeight"
* eaves height of building (base of roof structure, e.g the eaves against terrain): provided by BaseQuantity with Name="EavesHeight"

  
  
[<font color="#0000ff"><u>building_elevations</u></font>]($imageman://id=867057645;mdg=Global;name=building_elevations;type=Bitmap;)  
Figure 2 � Building elevations  
  
HISTORY New entity in IFC1.0.
