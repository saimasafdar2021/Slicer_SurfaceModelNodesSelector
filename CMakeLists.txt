cmake_minimum_required(VERSION 3.16.3...3.19.7 FATAL_ERROR)

project(SurfaceModelNodesSelector)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/saimasafdar2021/Slicer_SurfaceModelNodesSelector#readme")
set(EXTENSION_CATEGORY "Surface Models")
set(EXTENSION_CONTRIBUTORS "Saima Safdar (UWA)")
set(EXTENSION_DESCRIPTION "The module selects the nodes/vertices of each triangle in a surface modle and place a fiducial (3D point) at each vertex of each triangle in a surface model. The surface model can be any model.")
set(EXTENSION_ICONURL "https://raw.githubusercontent.com/saimasafdar2021/Slicer_SurfaceModelNodesSelector/main/SurfaceModelNodesSelector.png")
set(EXTENSION_SCREENSHOTURLS "https://raw.githubusercontent.com/saimasafdar2021/Slicer_SurfaceModelNodesSelector/main/sModel.png")
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
