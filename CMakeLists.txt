cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(SurfaceModelNodesSelector)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/SurfaceModelNodesSelector")
set(EXTENSION_CATEGORY "SurfaceModelNodesSelector")
set(EXTENSION_CONTRIBUTORS "Saima Safdar (UWA)")
set(EXTENSION_DESCRIPTION "This extensions selects the nodes/indexes of any surface model automatically. ")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/SurfaceModelNodesSelector.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/SurfaceModelNodesSelector/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(SurfaceModelNodesSelector)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})
