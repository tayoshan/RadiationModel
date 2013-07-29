RadiationModel
==============

Progress towards coding the radiation interaction model

Progress towards coding the radiation interaction model

-Utilizes numpy for scientific computing and matplotlib/networkx for visualization



-All distance calculation are based on euclidian distance despite the fact that the site's coordinates are
in decimal degrees. This was to have consistent units, since the the kd tree seems to be using euclidean distance. 
Using the haversine formula to calculate distances from the lat/long coordinates there does not match the 
kd tree indexing. The site's coordinates will likely need to be projected and transformed to meters to have
correct units and ensure consistency between the kd tree and inter-site ditances.
