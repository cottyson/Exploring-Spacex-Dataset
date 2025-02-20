### This repository focuses on the data scraping, data analysis, data preprocesing, data training and validation, and last but not least, data evaluation. Is there to note that there was no model deployment due to the academical purpose. The main porpuse of this repository is to review previous studies on data science, so there are some nootebooks that attend the same task but in different ways.

The firts step is to retrive the data, in this case this was done by two ways, one directly asking to the spacex API.  When this is done, the data tends to come in a format not fittable to work with, thats why there some features that
were discarted and otehr that were tranform, as is the case of "Core" which had as values a list of dictionaries ("jupyter-labs-spacex-data-collection-api"). The other way was making use of the BeatifullSoup library which facilitates the work  a lot.
making use of the tags of the HTML formats, is easy to extrac the info of the tables, but as in the first case, this formats tends to come in a not workable way, thats why there implemented some queries to extrac the desiered information. Is important 
to note that is very usufull to familiarize with the data one wants to fetch from the web before doing it("jupyter-labs-webscraping").


Once de data es obtained and stored in a DataFrame, we proceed to clean it("labs-jupyter-spacex-Data wrangling"). we dealt with the Nan values in the column "PayloadMass" by replacing them with the PayloadMass mean. In the case of "LandingPad" this values represent that no landingpad was used, hence the firststage did not land. we make use of the column "Outcome" to group all "True" outcomes and "False" outcomes so to create a binary class.


The NoteBook "jupyter-labs-eda-sql-coursera_sqllite-M2" focuses on the use of SQL lenguage for querying the Spacex data set, more concrete, the use of the inline magic commands. Aside of querying the data set, some feature enginering was perform, such as chanching the date from numbers to names.

Is of vital importance to analyse the data from a visual perspective, thats why in the NoteBook "edadataviz-M2" were used the seaborn and matplotlib libraries to create visualisations. we tried to find the relationships betwean some variables and the Successs result, as well yearly success rate since 2010.
