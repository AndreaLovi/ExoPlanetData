# ExoPlanetData
The Open Exoplanet Catalogue is a database of all discovered extra-solar planets. New planets are usually added within 24 hours of their announcement.  The database is licensed under an MIT license (see below), which basically says you can do everything with it. If you use it for a scientific publication, please include a reference to the Open Exoplanet Catalogue on github or to this arXiv paper.


Objectives of my Classworks are as follow: 

1. Import the dataset exo_data.csv as a tibble. Columns 1, 16, 17, 18, 25 should be
characters. Columns 2, 14 should be factors. Column 15 should be integers. The
remaining columns should be doubles.
Note: the file metadata.txt contains useful information about this dataset. Also,
you may consult https://en.wikipedia.org/wiki/Exoplanet

2. Exclude the exoplanets with an unknown method of discovery.

3. Create a graphic which illustrates the relationship between the log-distances from
the Sun and the methods of discovery.

4. Create scatterplots of the log-mass versus log-distances, separating by methods of
discovery. Hovering with the cursor highlights the point and displays its name, and,
if you click, the exoplanet’s page on the Open Exoplanet Catalogue will be opened.
(paste the id after http://www.openexoplanetcatalogue.com/planet/ ).

5. Rename the radius into jupiter_radius, and create a new column called earth_radius
which is 11.2 times the Jupiter radius.

6. Focus only on the rows where log-earth radius and log-period have no missing values,
and perform kmeans with four clusters on these two columns.

7. Add the clustering labels to the dataset through a new factor column called type,
with levels rocky, hot_jupiters, cold_gas_giants, others; similarly to https:
//en.wikipedia.org/wiki/Exoplanet#/media/File:ExoplanetPopulations-20170616.
png and produce the scatterplot highlighting these clusters.

8. Use a violin plot to illustrate how these clusters relate to the log-mass of the exoplanet.

9. Transform r_asc and decl into two new variables that are the same varibales but
in values of seconds. Use these as coordinates to represent a celestial map for the
exoplanets.

10. Create an animated time series where multiple lines illustrate the evolution over
time of the total number of exoplanets discovered for each method up to that year.
