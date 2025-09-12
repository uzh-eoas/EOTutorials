### Jupyter notebooks<br>
There are four Demo notebooks for you to explore:<br>
- Demo_Sentinel2_indices: Gives an overview of how you can work with a Sentinel-2 image that is already downloaded. This demo does not require you to have a GEE account.
- Demo_Sentinel2_indices_GEE: This demo works analogously to Demo_Sentinel2_indices but uses the GEE python API. It gives more information about the metadata of Sentinel-2 images.
- Demo_Sentinel2_timeseries_GEE: This demo is a continuation of Demo_Sentinel2_indices_GEE and calculates time series of different vegetation surfaces.
- Demo_Sentinel1_shipdetection_GEE: This demo gives an introduction to using Sentinel-1 SAR data to detect ships.  

### Installing the environment<br>
If you use Conda to manage your python packages and environments, you can use the provided gee_env.yaml to generate a new python environment. This allows you to run all four demo Jupyter notebooks.<br>

In the Anaconda prompt, change directory to the place where you stored the .yaml file (using cd). Then create the new environment using, this will take some time, as the environment has a large number of packages and dependencies.<br>

    conda env create -f gee_env.yaml 

In case of an error, it usually helps to clear the conda cache and try again:<br>

    conda clear --all 

After installing the environment, you can activate it using:<br>

    conda activate gee_env

The best way to use the provided Jupyter notebook is to use Jupyter Lab. This way, the interactive maps work the way they are intended. In e.g., PyCharm, the computations work fine, but the maps will not be displayed.<br>
Start Jupyter Lab using the Anaconda prompt:

    jupyter lab

You may have to navigate to the correct folder where you have stored the demo notebooks.

### Google Earth Engine<br>
To use the GEE Python APi, you need an active GEE account (which also requires a Gmail address). You can register a new Project here:<br>

    https://developers.google.com/earth-engine/guides/access

This page gives a good overview of how GEE works. The syntax of the Python API is a bit different from the native JavaScript used in the web-based GEE API, but the concepts are the same.

    https://developers.google.com/earth-engine/guides/getstarted
    
