# Using GIS in Python with Wreck Data

Code and presentation for the [NH Python meetup](https://www.meetup.com/New-Hampshire-Python-Group/events/qxqqtryccqbfc/) given December 2021:

> This month’s presentation with Heather Kusmierz is an introduction to working with geospatial data in Python using GeoPandas and folium. She'll introduce the basics of working with geospatial data including data models, common file formats, and some light theory on spatial reference systems and projections. Then she'll walk through a code demo to re-construct the search for a 100+-year-lost shipwreck that was discovered this summer by Eastern Search & Survey off the coast of Long Island, which will serve as a framework to demonstrate some common spatial analysis tasks.

The project uses an MIT license, which covers everything except the materials in the `data` folder. Datasets are saved there and retain their original use licenses. The image of the SS Biela on the cover of the presentation is copyrighted and used with permission by Ben Roberts, all rights reserved.

The code demo can be found in the `GIS_Analysis.ipynb` file.

The original project repository is located [here](https://github.com/Data-Science-for-Conservation/Ocean_GIS_for_Python).

## Create a Virtual Environment to Run the Code Locally

To run the Jupyter notebook locally, you'll need to create an environment with all the necessary packages and their dependencies.

To run with [Anaconda](https://www.anaconda.com/):

```shell
conda env create --file environment.yml

# Activate the new environment
conda activate geo

# Launch Jupyter notebooks
jupyter notebook
```

The code was only tested within an Anaconda environment, but there is a `requirements.txt` file if you would prefer to create the environment using PIP. Navigate to the project directory, then run the following commands. The `conda` environment uses Python 3.8.

```shell
# Create a virtual environment named "geo" in the project folder
python3 -m venv geo

# Activate the environment
source geo/bin/activate

# Install the packages via the requirements.txt file
python3 -m pip install -r requirements.txt

# Launch Jupyter notebooks
jupyter notebook
```
