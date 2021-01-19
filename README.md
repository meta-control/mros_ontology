# MROS T3 Metacontrol Ontologies

The purpose of MROS Task 3 is the development of an ontology to support metacontrol system modeling and run-time reasoning. These ontologies are used by the metacontroller implementation available [here](https://github.com/tud-cor/mc_mros_reasoner/tree/foxy_devel), note that the MROS reasoner used is in the branch _foxy-devel_.

## Overall view

The MROS objective is to use TOMASys concepts to implement a model-driven metacontroller for a ROS2 navigation system in two pilot robotic applications inside the RobMoSys framework.

The metacontroller will use a runtime reasoner that will exploit a system model to generate new runtime system configurations to overcome difficulties. This model and reasoner uses concepts that are reified in the form of an ontology captured in [Web Ontology Language v2](https://www.w3.org/TR/owl2-syntax/) (OWL 2).

The general ontology under development has been divided in two main parts: one dedicated to the navigation task — the focus of activity of both pilots— and another dedicated to the concepts related to system adaptation using the metacontrol approach. These two are known as Metacontrol Ontology (MO), and Navigation Ontology (NO).

Formal ontologies contain terms that capture the concepts in the domain of analysis. Ontologies attempt a formal naming and definition of the categories, properties and relations between the concepts, data and entities that populate a specifc domain of analysis.

## The Ontologies

The folder [**ontologies**](https://github.com/MROS-RobMoSys-ITP/metacontrol_ontology/tree/master/ontologies "MROS Ontologies") contains OWL2 files for the ontologies using OWL2 Functional Syntax. These files can be edited with any text editor or managed using a GUI-based tool like [Protégé](https://protege.stanford.edu/). The current structure is:

- **TOMASys**: General systems ontology for component organization to reach objectives through functions. Here is defined the terminological components (TBox) through classes, properties and general rules. This is equivalent to the previous Metacontrol Ontology .
- **MROS ontology**: TOMASys adaptation for MROS project ontology. TOMASys terminological components are extended with general error propagation rules and an object property to link components and function designs. Therefore, this ontology is the TBox that supports the specific pilot ontology. This is equivalent to the previous RobMoSys Ontology.
- **Navigation-domain ontology**: Basic application-specific knowledge regarding navigation concepts. Assertion components (ABox) have been generated for usual navigation applications based on ROS2. This is equivalent to the previous Navigation Ontology.
- **URJC Pilot ontology**: Ontology to capture application-specific knowledge, this is the assertion component (ABox). Here we define individuals and specific rules to transform the general knowledge of TOMASys into precise information for the pilot. 

Additionally a **TEST URJC** Pilot has been added for testing in Protege the ontology coherence.
