# ELA-calculation-toolbox

A GIS tool for automatic calculation of glacier equilibrium-line altitudes

Authors: Ramón Pellitero, Brice R. Rea, Matteo Spagnolo, Jostein Bakke, Susan Ivy-Ochs, Philip Hughes, Sven Lukas, Adriano Ribolini

Journal: Computers and Geosciences.

DOI: http://dx.doi.org/10.1016/j.cageo.2015.05.005

This is a tool for ELA calculation on glaciers with AAR and AABR methods. It has been developed using the arcpy library in Python 2.7. 
It runs in ArcGIS 10.1 and superior as a "toolbox". In this repository both the toolbox and the code that the tools run are available.
It consists of four different scripts:
- AABR (and AA): calculates the ELA Area-Altitude Balance Ratio for one raster glacier surface at a given ratio. Area-Altitude value is also calculated as an intermediate step.
- AAR (and MEG): calculates the ELA Area-Altitude Ratio for one raster glacier surface at a given ratio. Median Elevation of Glacier value is also calculated as an intermediate step.
- AAR (MEG) and AABR (AA) for several ratios. Performs the two previous calculations for a set of given ratios in one raster glacier surface.
- AAR and AABR (AA) several ratios and DEMs. Performs the two previous calculations for a set of given ratios in all the raster glacier surfaces stored in a folder.
Osmaston (2005) measurements for retrieving the best fit ratio in a group of glaciers are also calculated.

Outputs are shown either in the dialog window when running the tool (for the two first tools) or in a .txt (for the second tools). In all cases shapefile contour lines at the 
calculated altitudes are also output.

A model for raster surface creation from contour lines is offered too.

In order to use the tools just download the .tbx file and store it anywhere, open ArcGIS, open ArcToolbox, right click and select "Add Toolbox", the browse the tool in your system and select it. 

You can access the source code behind the tools by right clicking on them and selecting "Edit".
