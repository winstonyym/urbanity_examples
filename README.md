[![PyPI version](https://badge.fury.io/py/urbanity.svg)](https://badge.fury.io/py/urbanity)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/urbanity)](https://badge.fury.io/py/urbanity)
[![Documentation Status](https://img.shields.io/readthedocs/urbanity)](https://urbanity.readthedocs.io/)
# Urbanity

**Urbanity** is a network-based Python package to automate the construction of feature rich (contextual and semantic) urban networks at any geographical scale. Through an accessible and simple to use interface, users can request heterogeneous urban information such as street view imagery, building morphology, population (including sub-group), and points of interest for target areas of interest. 

If you use Urbanity in your work, please cite:
(*Urbanity is currently under review.*)
## Purpose
This repository provides a guide to getting started and implementing some of the basic functionalities and analytical tasks outlined in the [example notebooks](https://urbanity.readthedocs.io/en/latest/index.html#). 


## Quickstart
*How do I get started?*

First, clone this repository and the sample data files provided. The repository is organised as follows:

πurbanity <br/>
 β£ πAGGREGATE_STATS <br/>
 β- β bangkok_stats.csv <br/>
 β- β bangkok_subzone_stats.csv <br/>
 β  ... <br/>
 β£ πdata <br/>
 β- β new-york-latest.osm.pbf <br/>
 β- β Seattle.osm.pbf <br/>
    ... <br/>
 β£ πfigures <br/>
 β- β output.png  <br/>
 β  ... <br/>
 β£ πGUN <br/>
 β- β bangkok100m.csv <br/>
 β- β bangkok100m.geojson <br/>
 β- β bangkok200m.csv <br/>
 β- β bangkok200m.geojson <br/>
 β- β chicago100m.csv <br/>
 β- β chicago100m.geojson <br/>
 β- β chicago200m.csv <br/>
 β- β chicago200m.geojson <br/>
 β  ... <br/>
 β£ πSHAPEFILES <br/>
 β- β bangkok.geojson   <br/>
 β- β seattle_subzones.geojson  <br/>
    ...  <br/>

`AGGREGATE_STATS` provides computed aggregate indicators for cities and their subzones.  <br/>
`data` is the location where downloaded osm.pbf files are stored. <br/>
`figures` specifies where plots generated from notebook examples should be placed.   <br/>
`GUN` provides pre-computed node and edge attribute features for various cities. <br/>
`SHAPEFILES` includes some polygon shapefiles that were used to specify geographical boundaries. <br/>

### Step 1:
Navigate to a location of choice (e.g., Desktop or project folder).

### Step 2:
Clone the repository from github or directly download the zip file and place it at the location of choice (Step 1).

### Step 3: 
3) Open up a terminal/command prompt and input the following command:

```Terminal
$ conda env create -f environment.yml
$ conda activate urbanity
```

(Optional) For JupyterLab / JupyterNotebook users, you can additionally add a notebook kernel via:

```Terminal
$ python -m ipykernel install --user --name=urbanity
$ jupyter lab
```
### Step 4: 
4) Installation completed and you should be able to use urbanity and follow along with the example notebook without issues.


Detailed documentation is available at [documentation](https://urbanity.readthedocs.io/).
## License

`urbanity` was created by winstonyym. It is licensed under the terms of the MIT license.