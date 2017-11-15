# Midterm Project CFF Railway network

In this folder you can find all the data and analysis done for the Midterm Project on the CFF Railway Network. I've extracted all the data from the following website https://opentransportdata.swiss/fr/dataset/timetable-2017-gtfs. It gives all the data for upcoming trips in Switzerland for the next coming year from 10th of December 2017 to 8th of December 2018. To have a better view of how the data are organized, please take a look at the UML diagram which show the structure and the architecture of it. 

IMPORTANT : As the size of the data is really important (more than 4 000 000 lines in some files), the cleaning notebooks take really long time to execute. I advise therefore not to run these notebook but run only the "Network Analysis" one which import directly the .gml graph and analyze it. 

Here are some informatioon on the structure of the project and how the data were cleaned and analyzed:
  - The .txt files are the original files I've downloaded from the website. The .csv, .xlsx, .gml are created through the cleaning notebooks. 
  - The files "stop_times" and "trips" are Zipped because of the large size of the file. 
  - The UML diagramm in PNG format shows the architecture of the data.
  - There are three different notebook in the repository. "Data cleaning" and "Data cleaning 2" show how I cleaned the data from the .txt files and created the graph  and the "Network analysis" shows all the analysis conducted on the generated network. It covers all the aspects seen so far in the course. For the cleaning part, I've decided to only consider train data and only some features among all available. I've created some .csv file to stock the useful data. Once all the useful data are stocked, I've created the graph CFF_Graph and stock it in a .gml file for future analysis. In the analysis notebook, I import the .gml graph generated before and analyze it. 
  - Some additional data are available in the ZIP file "Additional data". It contains different calendar and transfer details not useful for the first analysis conducted in this MidTerm project. It might be useful for the final project. 
  
 Finally, due to time constraints, some parts like the homophily one is not really detailed but I will be more than happy to continue to explore this network for the final project.
