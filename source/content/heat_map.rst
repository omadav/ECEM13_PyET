
.. _heatmap:

******************************************************************
Fixation Distribution Using Heat Map Visualization
******************************************************************

The basic steps involved in Fixation Distribution Using Heat Map Visualization
using eye data from the ioDataStore:

X. Load the eye data from the ioDataStore (in this example we will just create simulated fixation data to spare time).
A. Define settings to control how fixation data is used to great the heat map, and how the heat map should look.
B. Create 2D Gaussian Mask templateto use as the fixation denisity map for each fixation being used.
C. Load the background image displayed during eye data collection.
D. In our example, create some random fixation data.
E. Create the fixation density map based on the variable values specified in A, the gaussian created in B., and the Fixation data either loaded in X., or in our case, created in D.
F. Turn the fixation density map into a heat map by applying a color range to the fixation map data.
G. (Optional) Create a figure plotting

    # Gausian mask being used.
    # Background image the heatmap will be applied to.
    # The fixation data points used in creating the fixation density map.
    # The heat map created which will be overlayed on the background image.

H. Create the final fixation denisity based heat map overlayed on the background image. 

.. literalinclude:: python_source/data_visualization/heat_map.py
    :language: python

Example Plots
------------------

Components used in creating a fixation density based heat map.

.. image:: ./heat_map_components.png
    :width: 700px
    :align: center
    :height: 500px
    :alt: Components used in creating a fixation density based heat map.
    

The final heat map result.

.. image:: ./heat_map.png
    :width: 700px
    :align: center
    :height: 500px
    :alt: The final heat map result