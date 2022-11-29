# Virtual-Real-Integration

This repository is for exploration of [use cases](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/readme.md) (UCs) for Real/Virtual World integration. 

The first use case (UC1), [Assisted Car-Human Urban Rendezvous](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/UC1/readme.md) is based on the general ideas of the "shared ride arriving for a passenger pickup scenario" that we have talked about off and on in the meetings. 

The second use case (UC2), [Underground Utilities - Reading the Street](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC2) is based on the need to understand what is buried in the ground at a construction site before and during excavations in order to prevent damage and injury. The location of buried pipes and cables are often only known approximately until they are exposed during digging. As they are exposed and as new facilities are placed in an excavation prior to burial, it is possible to make accurate surveys of 3D location. 

## Plan



1. **EG Chairs**: Seed the process with a starting version of UC1. To start this, I (Steve) am reverse-engineering parts of our first 6 meetings to create a complete and internally consistent version of UC1, [James Jackson's Building Blocks](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/buildingblocks#readme) (BB) including more detailled physical and semantic element classes (SECs) of UC1.  The latter are the "Reality Players" of James Jackson's slide. We can begin the collaboration with a more or less **complete** and internally consistent starting set of semantic element classes (SEC) of a "Use Case World" (UCW) targeting just UC1.

2. **Collaboratively**: add service interfaces (SI) to James Jackson's Building Blocks (BBs) and to SECs to allow instances of the SECs to carry out UC1. The result could be (a) a graph with SECs and BBs as nodes and SIs as edges, and (b) a time sequence along the lines of a UML sequence diagram. This graph could be encoded in the DOT language, which is editable and viewable [online](https://github.com/magjac/graphviz-visual-editor) . Links will go in the *tools* folder.

3. **Collaboratively**: evolve the UC1 graph to reach a consensus structure for UC1. Both semantic classes and interfaces (i.e. everything) can be changed here.

4. **Collectively**: decide whether to adopt the consensus UC1 graph as the basis of a Working Group for developing a prototype of UC1 to demonstrate the possible use of existing standards and gap-filling additional standards to implement Real/Virtual World Integration in a technically realisable metaverse. 

## Next Steps

Please raise issues reflecting your needs, opinions, ideas, both on the above plan and the choice of UC1.

Completed the "seeding" 27 November 2022. This provides a few days before our next EG meeting on 1 December 2022 to move on to step 2 of the plan.

As of November 27th, the [Building Blocks](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/buildingblocks#readme), the [basic schema](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1/world) , [use case description](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1#readme) , [action sequence](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1/sequence#readme) , and [markdown manifest](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/UC1/world/integrated/integrated.md) of a populated example integrated world for Use Case 1 are in place. 
