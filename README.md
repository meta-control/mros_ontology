# MROS T3 Metacontrol Ontologies

The purpose of MROS Task 3 is the development of an ontology to support metacontrol system modeling and run-time reasoning.

## Overall view

The MROS objective is to use TOMASys [^1] concepts to implement a model-driven metacontroller for a ROS2 navigation system in two pilot robotic applications inside the RobMoSys framework.

The metacontroller will use a runtime reasoner that will exploit a system model to generate new runtime system configurations to overcome difficulties. This model and reasoner uses concepts that are reified in the form of an ontology captured in [Web Ontology Language v2](https://www.w3.org/TR/owl2-syntax/) (OWL 2).

The general ontology under development has been divided in two main parts: one dedicated to the navigation task — the focus of activity of both pilots— and another dedicated to the concepts related to system adaptation using the metacontrol approach. These two are known as Metacontrol Ontology (MO), and Navigation Ontology (NO).

Formal ontologies contain terms that capture the concepts in the domain of analysis. Ontologies attempt a formal naming and definition of the categories, properties and relations between the concepts, data and entities that populate a specifc domain of analysis.

## The Ontologies

The folder [**ontologies**](https://github.com/MROS-RobMoSys-ITP/metacontrol_ontology/tree/master/ontologies "MROS Ontologies") contains OWL2 files for the ontologies using OWL2 Functional Syntax. These files can be edited with any text editor or managed using a GUI-based tool like [Protégé](https://protege.stanford.edu/).
