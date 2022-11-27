# Virtual-Real-Integration

This repository is for exploration of use cases (UCs) for Real/Virtual World integration. 

The first use case (UC1), [Assisted Car-Human Urban Rendezvous](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/UC1/readme.md) is based on the general ideas of the "shared ride arriving for a passenger pickup scenario" that we have talked about off and on in the meetings. 

## Initial Plan



1. **EG Chairs**: Seed the process with a starting version of UC1. To do this, I am reverse-engineering parts of our first 6 meetings to create a complete and internally consistent version of UC1, [James Jackson's Building Blocks](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/buildingblocks#readme) (BB) including more detailled physical and semantic element classes (SECs) of UC1.  The latter are the "Reality Players" of James Jackson's slide. I want to start the collaboration with a **complete** and internally consistent starting set of semantic element classes (SEC) of a "Use Case World" (UCW) targeting just UC1.

2. **Collaboratively**: add service interfaces (SI) to James Jackson's Building Blocks (BBs) and to SECs to allow instances of the SECs to carry out UC1. The result could be (a) a graph with SECs and BBs as nodes and SIs as edges, and (b) a time sequence along the lines of a UML sequence diagram. This graph could be encoded in the DOT language, which is editable and viewable [online](https://github.com/magjac/graphviz-visual-editor) . Links will go in the *tools* folder.

3. **Collaboratively**: evolve the UC1 graph to reach a consensus structure for UC1. Both semantic classes and interfaces (i.e. everything) can be changed here.

4. **Collectively**: decide whether to adopt the consensus UC1 graph as the basis of a Working Group for developing a prototype of UC1 to demonstrate the possible use of existing standards and gap-filling additional standards to implement Real/Virtual World Integration in a technically realisable metaverse. 

## Next Steps

Please raise issues reflecting your needs, opinions, ideas, both on the above plan and the choice of UC1.

My target is to complete the "seeding" by 27 November 2022. This will provide a few days before our next EG meeting on 1 December 2022 to move on to step 2 of the plan.

As of November 27th, the [Building Blocks](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/buildingblocks#readme), the [basic schema](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1/world) , [use case description](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1#readme) , [action sequence](https://github.com/MetaverseStandards/Virtual-Real-Integration/tree/main/src/UC1/sequence#readme) , and [markdown manifest](https://github.com/MetaverseStandards/Virtual-Real-Integration/blob/main/src/UC1/world/integrated/integrated.md) of a populated example integrated world for Use Case 1 are in place. To come in the next few days:

- JSON manifest for integrated world - may become issue
- semantic schema as DOT file - may become issue
- create issue for developing corresponding interfaces connecting Building Blocks in the "Omniverse" to the integrated world (metaverse?).

