#----------------------------------------------------------------------------
# Setup the project
cmake_minimum_required(VERSION 2.6 FATAL_ERROR)
project(Geant4GarfieldDegradInterface)

add_subdirectory(Xenon)
add_subdirectory(ALICE)

add_custom_target(Interface DEPENDS Xenon ALICE)
