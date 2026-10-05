# SRTO Ontology Engineering 
The ontology engineering process usually involves multiple steps. The first step is to define a set of competency questions. The SRTO ontology aims to answer some of the following example questions: 
- Can you provide the route between A and B? 
- What are adjacent nodes to a particular node? 
- Show me all the intersections where I can turn, right ? 
- What is the speed limit on a particular road? 
- What is the maximum flow over the particular road? 
- What are the roads that allow trucks during the night? 
- Which road segment meets at a particular junction? 
- Which lane should I turn left? 
- What is the speed limit on a particular road at a specific time?  
## Distinguishing Topology and Geometry representation 
The second step involves designing an ontology that models the real-world domain. In this case, an important aspect is to distinguish transport network topology concepts, such as nodes and arcs, from the physical and geometric representations of the transport network, such as intersections, junctions, and road segments.For geometric representations, we reuse the GeoSPARQL ontology and its classes for representing different spatial objects using geometries such as points and lines. For topological concepts, we introduce two new classes: *Arc* and *Node*.
## Adding restrictions
Next step is to add different type of restictions for routing through transpprt network. We introduced a new class Restriction andseveral object properties hasTurnRestriction, hasAccessRestriction and other. 
