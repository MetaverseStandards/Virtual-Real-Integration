# Virtual-Real-Integration

This repository is for exploration of [use cases](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/readme.md) (UCs) for Real/Virtual World integration. 

The first use case (UC1), [Assisted Car-Human Urban Rendezvous](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/UC1/readme.md) is based on the general ideas of the "shared ride arriving for a passenger pickup scenario" that we have talked about off and on in the meetings. 

The second use case (UC2), [Underground Utilities - Reading the Street](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC2) is based on the need to understand what is buried in the ground at a construction site before and during excavations in order to prevent damage and injury. The location of buried pipes and cables are often only known  to different levels of precision as the design and excavation proceed
1. During the design phase there may be either general records of a buried pipe or cable but only within a wide corridor _or_ there may be "as-built" video or imagery that can be used to provide an integrated view beneath the ground surface.
2. During the location phase, the horizontal precision may be improved to a few tens of centimeters horizontally and a half meter vertically.
3. During excavation, the precise location and condition is exposed within the excavated area.
The integrated virtual/real view can be updated as the work proceeds to provide the best-available information as the work proceeds. Since very approximate information may be replaced by direct observation of the initially hidden buried facilities, it is possible to update the model based on these "as-built" observations so that they may be integrated into a view if a later project involves the same buried objects.
 

## Plan



1. **EG Chairs**: Seed the process with a starting version of UC1. To start this, I (Steve) am reverse-engineering parts of our first 6 meetings to create a complete and internally consistent version of UC1, [James Jackson's Building Blocks](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/buildingblocks#readme) (BB) including more detailled physical and semantic element classes (SECs) of UC1.  The latter are the "Reality Players" of James Jackson's slide. We can begin the collaboration with a more or less **complete** and internally consistent starting set of semantic element classes (SEC) of a "Use Case World" (UCW) targeting just UC1.

2. **Collaboratively**: add service interfaces (SI) to James Jackson's Building Blocks (BBs) and to SECs to allow instances of the SECs to carry out UC1.  

3. **Collaboratively**: evolve the UC1 graph to reach a consensus structure for UC1. Both semantic classes and interfaces (i.e. everything) can be changed here.

4. **Collectively**: decide whether to adopt the consensus UC1 graph as the basis of a Working Group for developing a prototype of UC1 to demonstrate the possible use of existing standards and gap-filling additional standards to implement Real/Virtual World Integration in a technically realisable metaverse. 

## Next Steps

Please raise issues reflecting your needs, opinions, ideas, both on the above plan and the choice of UC1.

The [Building Blocks](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/buildingblocks#readme), the [basic schema](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1/world) , [use case description](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1#readme) , [action sequence](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1/sequence#readme) , and [markdown manifest](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/UC1/world/integrated/integrated.md) of a populated example integrated world for Use Case 1 are in place. 
