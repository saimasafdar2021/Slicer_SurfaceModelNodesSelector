# SurfaceModelNodesSelector

The module selects the nodes/vertices of each triangle in a surface modle and place a fiducial (3D point) at each vertex of each triangl ein a surface model.
The surface model can be any model. 

It takes the directory for which
  it looks for the .ply files the model files
  keep track of all the files in a folder that is provided 
  and then make the json markups file for each model and saves it in the same directory with the corresponding model name,

Input: input is the folder containing the .ply model files
Output: output contains all the json files for all the models (.ply models)

Model with selected surface nodes/vertices of each triangle in a model
![sModel](https://github.com/saimasafdar2021/Slicer_SurfaceModelNodesSelector/assets/80670821/7d3f869d-f6e0-4431-979c-d28fe72a751f)


To run using command line in linux:
./Slicer --python-script /path/to/script/surfaceModel.py --no-main-window

on mac:
/applications/Slicer.app/contents/MacOS/Slicer --no-main-window --no-splash --python-script "/full/path/toscript/surfaceModel.py"
