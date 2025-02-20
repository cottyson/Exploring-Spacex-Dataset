### This repository focuses on the data scraping, data analysis, data preprocesing, data training and validation, and last but not least, data evaluation. Is there to note that there was no model deployment due to the academical purpose.

The firts step is to retrive the data, in this case this was done by two ways, one directly asking to the spacex API.  When this is done, the data tends to come in a format not fittable to work with, thats why there some features that
were discarted and otehr that were tranform, as is the case of "Core" which had as values a list of dictionaries ("jupyter-labs-spacex-data-collection-api"). The other way was making use of the BeatifullSoup library which facilitates the work  a lot.
making use of the tags of the HTML formats, is easy to extrac the info of the tables, but as in the first case, this formats tends to come in a not workable way, thats why there implemented some queries to extrac the desiered information. Is important 
to note that is very usufull to familiarize with the data one wants to fetch from the web before doing it("jupyter-labs-webscraping").
