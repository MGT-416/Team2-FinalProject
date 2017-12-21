# Final Project CFF Railway network
## Clement Catajar, Cedric Cook

In this folder you can find all the data and analysis done for the Final Project on the CFF Railway Network. The data used to generate the network were taken from https://opentransportdata.swiss/fr/datasetList. It contains all the information on the transportation data in Switzerland. For this analysis we used the train and bus schedule for the coming year 2018.

In this project, we will explore the CFF railway and busses network to find the spreading of a virus and the most influential spreaders. We will analyze this phenomenon with a modified SIR model. Indeed, based on the basic SIR infection model, we will attribute a probability of infection proportional to the population of the city and the type of stops (bus or train stop) and determine the most influential spreaders among all the cities in Switzerland.

This project aims to answer the following questions:

- What is the percentage of Switzerland's population attained when a virus is spread from a Swiss city?
- What are the most critical starting cities for infection?

The work on these questions was done in different parts. First of all, it was necessary to acquire all the data for the network and prepare it for further analysis. Then the analysis was done in two main parts, the first one was the computation of the main basic and centrality measures in order to understand the network's behavior and secondly we built a modified SIR model to evaluate the spread of an infection in the network.

IMPORTANT : As the size of the data is really important (almost 4 000 000 lines in some files), the cleaning and analysis notebooks take really long time to execute. 

Here are some informatioon on the structure of the project and how the data were cleaned and analyzed:
  - The final project notebook contains all the analysis, comments and conclusion on the project. 
  - The folder data_cleaning contains all the notebooks and useful files to prepare the data. The main notebook Data Cleaning Final contains four main parts : 
    - Identification of the relevant routes, trips and stops
    - Identification of trips sequence
    - Population preparation
    - Network generation with attributes
  - The UML diagramm in PNG format shows the architecture of the data.
  - The CFF_Graph contains only the trains and the CFF_Graph_Final_3 contains also the busses.
  - The notebook "Network analysis final" contains all the code for the analysis. It is the same code as the one included in the report.
