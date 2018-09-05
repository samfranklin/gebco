Gebco
---

## Introduction

This repository contains scripts and (some data) for using the "pydata stack" to read, process and visulise global bathymetry data from the Gebco project. The aim of this project is to use python libraries together with a Jupyter Notebook instead of the traditionally desktop GIS application for reading, manipulating and visualising geospatial data. The pydata stack is a particularly powerful set of libraries and frameworks that are now challenging traditional applicaiton-specific workflows.

As well as using the libraries, I'm going to spend some time on setting up the python environment, as this is a big barrier for no or limited software development experience to get started.

Who is aimed at?  
Anyone interested in python and geospatial data processing or visualisation. I spent a number of years being confused or indeed scared of "messing" with python for fear of breaking something. Hopefully, this "HowTo" will shed some light on the process. If your comfortable with setting up your environment, please skip ahead to the notebook

Jump to to the [Jupyter Notebook](gebco-read-viz.ipynb)

## Requirements
The software packages needed for running this jupyter notebook.
* Jupyter Notebook - a framework for running python code directly in your web browser
* xarray - a python package for working with NetCDF data
* matplotlib - a python package for making plots and charts
* cartopy - a python package that works with matplotlib, specifically for geographic data
* seaborn - a python package that works with matplotlib, but provides nicer graphics

## Build Process
The short answer is that we will create a python environment using some software called "anaconda".
Anaconda is a software application that provides the user with the ability to create "virtual" python environments that should not mess with other python environments that you could be using e.g. your "system python" (the python version that is shipped with OSX or Linux/GNU) or any other python environment, e.g. if you use Windows and you have Python packaged with OSGeo or ArcGIS. The mistake I made in the past was thinking that surely I have one single python environment that works for all software packages. I've found it's preferable to have discrete managed python instances that do not conflict. This is where anaconda comes in.

### Working on Windows:
* To be completed

### Working on OSX
* To be completed

### Working on GNU/Linux
* To be completed

### Data Source
* Data sourced from Gebco [here](https://www.gebco.net/data_and_products/gridded_bathymetry_data/)

## ToDo:
* add a save to netcdf file using xarray
* add a netcdf to GTiff export using rasterio.
* add seaborn palette change
* interplote a dem profile between to arbitary points that is not aligned with the grid
* interpolate a dem profile along an input linestring geometry e.g. a boat transect from a geoJSON
* if the file is too big for memory use dask
* migrate the dataset to a multi-variable, multi-timestep netcdf e.g. model output from NOAA Wave Watch 3.
