cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(ElectronBolus)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/ElectronBolus")
set(EXTENSION_CONTRIBUTORS "Sima Azhari (Mashhad University of Medical Sciences), Csaba Pinter (EBATINCA)")
set(EXTENSION_DESCRIPTION "This extension generates a bolus for electron radiation therapy to shape the dose distribution for a given target.")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/ElectronBolus.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/ElectronBolus/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(ElectronBolus)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
