# COncORDE incident model

#Introduction
In COncORDE project incident information is represented with flexible ontological model that can be served as an intelligent context-aware semantic data store for the Incident related information [1].  Core concepts of incident model can be categorized with a vocabulary based on EDXL standard that provides various categorizations for concepts such as types of incidents and resources and organization participating it (https://github.com/OntoRep/EDXL). Incident model is aligned with PROV-O ontology so that it supprots decision making by modelling by who, by which activity, when and based on which information the decisions was made [2].

##Visualization of current status
This document provides diagrams generated from Enterprice Architect ODM plugin and Protege OntoGraph plug-in, those may not reflect the latest status of vocaubulary. A visualization of current snapshot of vocabulary can be found from:

[WEBOWL online visualization of current snapshot of ontology.](http://vowl.visualdataweb.org/webvowl/#iri=https://raw.githubusercontent.com/OntoRep/COncORDE/master/concorde.ttl "WEBOWL visualization")


#Overview of ontology

Main ontology classes for modelling incidents is presented in following diagram.

![Incident model](https://raw.githubusercontent.com/OntoRep/COncORDE/master/EA8.png)

Incident is the core class that links together different knowledge elements and defines the main data structure of an emergency incident. As Incident can be associated with data from different sources that provide information about an emergency incident. The Incident model reuses various state of the art extenral ontologies such as ‘time:TemporalEntity’ and ‘geo:SpatialEntity’ concepts that are used to define start and end times and geographical locations of an incident.  The Incident core ontology is also aligned with PROV ontology so that the Role, Entity and Activity concepts are reused (sub-class relations classes not included into the diagram, are shown in the upper right corner of the boxes)

Modelling of incident participants is shown in the next diagram. Participant class models various emergency response related roles and actors are associated to a specific incident individual.  

![Participants](https://raw.githubusercontent.com/OntoRep/COncORDE/master/EA12.png)

Resource class models participants needed for accomplishing different assignments in an emergency response scenario. COncCORDE incident ontology provides provides vocabularies for defining specific activities required by roles and matching thoses of profiles of persons and organization (i.e. agents) identified in the COncORDE project but not covered by EDXL standard. 

![Participants](https://raw.githubusercontent.com/OntoRep/COncORDE/master/EA16.png)

Incident ontology also provides simple vocabulaires for environmental information such as weather using similar approach than EDXL vocabulary.

#References
[1] COncORDE D3.3 Development of Coordination Mechanisms During Different Kinds of Emergencies

[2] COncORDE D3.4 Situational awareness and joint decision support
