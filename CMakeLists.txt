cmake_minimum_required(VERSION 3.5)
project(mros_ontology)

find_package(ament_cmake REQUIRED)

set(mros_ontology_MAJOR_VERSION 0)
set(mros_ontology_MINOR_VERSION 1)
set(mros_ontology_PATCH_VERSION 0)
set(mros_ontology_VERSION
  ${mros_ontology_MAJOR_VERSION}.${mros_ontology_MINOR_VERSION}.${mros_ontology_PATCH_VERSION})

# launch
install(DIRECTORY ontology DESTINATION share/${PROJECT_NAME})

ament_package()
