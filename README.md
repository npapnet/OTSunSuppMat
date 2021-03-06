## Supplementary files for: 
# "OTSun, a Python package for the optical analysis of solar-thermal collectors and photovoltaic cells with arbitrary geometry"
## By Gabriel Cardona and Ramon Pujol

The requirements to run these scripts are python 3.6 with the library `otsun` installed (can be installed via `pip`), together with the FreeCAD libray. For convenience of the reader, a `Vagrantfile` is provided, which together with `bootstrap.sh` can be used by [vagrant](https://www.vagrantup.com/) to create a virtual machine with all the requirements installed.

The included files and folders are:

* `ParabolicTrough.FCStd`: FreeCAD file showing how materials are identified by the labels of the objects.
* `validation1.py`: Script used to make the computations for the first validation of OTSun in the main paper.
* `LFR.FCStd`: FreeCAD file defining the geometry of the optical system used in `validation1.py`.
* `LFR.tnh`: Tonatiuh file defining the same geometry as in `LFR.FCStd`
* `LFR_output.FCStd`: FreeCAD file obtained as output by OTSun with some simulated rays.
* `validation2.py`: Script used to make the computations for the second validation of OTSun in the main paper.
* `mirror.FCStd`: FreeCAD file defining the geometry of the optical system used in `validation2.py`.
* `mirror_output.FCStd`: FreeCAD file obtained as output by OTSun with some simulated rays.
* `data`: Folder with data for specification of parametric materials and solar spectrum.
* `output1` and `output2`: Folders with the outputs of `validation1.py` and `validation2.py`, respectively.

To reproduce the computations, simply run the scripts `validation1.py` and `validation2.py`. Note that this will overwrite the contents of the folders `output1` and `output2`, respectively.
