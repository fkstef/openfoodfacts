## OpenFoodFacts data analysis

The repository you are looking as is a data science project.
The main content is a Python notebook that handles data loading, transformation, 


## Installation <a name="installation"></a>

The additional libraries on top of the standard distribution of Python 3.* necessary are:
- pandas: https://pandas.pydata.org/ (necessary to process all dataframes operations)
- numpy: https://numpy.org/ (used for some data transformations and calculations)
- matplotlib: https://matplotlib.org/ (for data visualisation)
- seaborn: https://seaborn.pydata.org/ (for data visualisations)
- geopandas: http://geopandas.org/ (to build the world map visualisations)
- pycountry: https://pypi.org/project/pycountry/ (used as a reference database for country names and ISO codes)
- scikit-learn: https://scikit-learn.org/stable/ (used for machine learning algorithms, namely random forest classifications)


## Project Motivation<a name="motivation"></a>

For this project, I was interestested in analysing some features of the OpenFoodFacts data available from https://world.openfoodfacts.org/data and understand the geographical information and nutritional information that it contains.

I was also interested in combining this information with additional data sources, such as the worldbank life eexpectancy data. I wanted to identify if the product selection per country and nutritional value (measured through the nutri-score) was in any way correlated with the health of the population (measured through life expectancy).


## File Descriptions <a name="files"></a>

The main file in the repository is openfoodfacts.ipynb which is the python notebook to reproduce the calculations and generate the visualisations. The first set of notebook cells will download additional data not included in this repository. These have been marked in the git exclusion list in the .gitignore file.


## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@stephaneschitter/https-medium-com-stephaneschitter-should-you-eat-that-food-234ba2bf240).

The notebook shows that the majority of the openfoodfacts database is made of products sold in France. Products available in other countries are present in the database but with a much lower representativity. Quality of data is not exceptional, probably mainly due to to the crowdsourcing as the primary creation mechanism of new data.

This project also shows that it is possible to calculate the nutri-score using a random forest classifier with almost 90% accuracy based only on nutrients information. Finally, the data available does not show a correlation between the nutri-score of products sold in a country and life expectancy in the same country. This does not mean the two statistics are not correlated, but the quality and quantity of data available was not sufficient to demonstrate any link.


## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Credits go to OpenFoodFacts for making the data available and the platform for users to contribute. You can find the Licensing for the data and other descriptive information at the link available [here](https://world.openfoodfacts.org/data).

Credits also go to Worldbank for making world development data available. Licensing for the worldbank datasets is available [here](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets).

Feel free to use the code from the notebook for your own purposes.
