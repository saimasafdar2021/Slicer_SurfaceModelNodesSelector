# SurfaceModelNodesSelector

## Description 
The module selects the nodes/vertices of each triangle in a surface modle and place a fiducial (3D point) at each vertex of each triangl ein a surface model.
The surface model can be any model. 

## How to use it?
It takes the directory for which
  it looks for the .ply files the model files
  keep track of all the files in a folder that is provided 
  and then make the json markups file for each model and saves it in the same directory with the corresponding model name.

Input: input is the folder containing the .ply model files
Output: output contains all the json files for all the models (.ply models)

## Example Output
Model with selected surface nodes/vertices of each triangle in a model
![sModel](https://github.com/saimasafdar2021/Slicer_SurfaceModelNodesSelector/assets/80670821/7d3f869d-f6e0-4431-979c-d28fe72a751f)

## Running through terminal
To run using command line in linux:
./Slicer --python-script /path/to/script/surfaceModel.py --no-main-window

on mac:
/applications/Slicer.app/contents/MacOS/Slicer --no-main-window --no-splash --python-script "/full/path/toscript/surfaceModel.py"
## surfaceModel.py file 
s = slicer.modules.surfacemodelnodesselector.widgetRepresentation().self().logic.process("/media/useradmin/Disk2/Slicer-5.3.0-2023-01-21-linux-amd64/25_manually_picking_points/25_manually_picking_points/")
