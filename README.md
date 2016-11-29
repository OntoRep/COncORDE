# COncORDE incident and context ontologies

#Introduction
In COncORDE project incident information is represented with flexible ontological model that can be served as an intelligent context-aware semantic data store for the Incident related information [1].  

#Overview of ontology

Main ontology classes for modelling incidents is presented in following diagram.

![Report categories](https://raw.githubusercontent.com/OntoRep/COncORDE/master/EA8.png)

Incident is the core class that links together different knowledge elements and defines the main data structure of an emergency incident. As Incident can be associated with data from different sources that provide information about an emergency incident. 

Participant class models various emergency response related roles and actors are associated to a specific incident individual. The Incident model reuses various state of the art extenral ontologies such as ‘time:TemporalEntity’ and ‘geo:SpatialEntity’ concepts that are used to define start and end times and geographical locations of an incident. 

The Incident core ontology is also aligned with PROV ontology so that the Role, Entity and Activity concepts are reused (sub-class relations classes not included into the diagram, are shown in the upper right corner of the boxes)-

#References
[1] COncORDE D3.3 Development of Coordination Mechanisms During Different Kinds of Emergencies
[2] COncORDE D3.4 Situational awareness and joint decision support
