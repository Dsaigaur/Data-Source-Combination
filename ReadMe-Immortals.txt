
The is a capstone project which aims to analyse the accident/incident/failure of Aviation data.


OVERVIEW OF THE PROJECT

The Aviation data sources are used to document an aircraft incident,accident, or failure.The subject matter experts
who create a data entry have different perspectives. The objectives are specific to their line of business. The data 
systems are not connected.Insight will improve with a more complete picture of any incident.

The project is scoped as a merging project and find insights to understand the accidents and help manage incidents better. These incidents are reported every time an unusual incident occurred during civil flights. 
Although, the repositories consist of routine problems, they are a valuable source of information about possible sources of prominent dangers. 
There was no previous work done to consolidate the multiple reports to create a concise report. Merged data created will help in solving different kinds of problems which deal with safety measures that have to be taken into consideration to avoid previously occurred incidents.
The model uses the 2019 accident/incident data.  

The analytical approach of model uses advanced NLP (Natural language processing) techniques and Latent Dirichlet Allocation (LDA) (topic modelling) to extract useful information from the reported incidents using Python.
The results have shown very good potential to help the Federal Aviation Administration (FAA) in their further analysis.

The datasets provided are SDRS (Service Difficulty Reports) , AID (Accident/Incident Data) and EON data.
As said above, these datasets are written with different perspectives.

CODE

In the files given, 'Initial FAA Analysis' was our first approach to the analysis of the AID,SDRS,EON data cleaning and merge these datasets.
'Data pre-processing and merging' shows the final approach of the data-preprocessing and obtained the merged of all the datsets.(this showed better results compared to the initial analysis)
'Project_FAA_topic modelling'. We took the merged data and did further analysis on the data. It mainly involved the topic modelling using LDA and finding the best category for any given incident.
'Visualization' is a powerpoint file consists of all the visualizations created using tableau tool.(We're still working on this phase of the project).
All the remaining Initial NLP files gave us a better understanding of the categorical data.


HOW IT WAS DONE?

The initial phase, Data gathering,understanding and cleaning the domain took us little more than expected as there are many number of columns,terms and definitions to understand from the data.
The data given is messy and not a straight forward one. There are lot of columns with inconsistancies,NA values,poor format etc. It took us time to filter the attributes/columns which are beneficial for the project.
Data quality checks and validation is an important step in this phase.
Each dataset required different methods for the cleaning as there are from different repositories. Finally, the datasets SDRS,AID and EON are merged after the cleaning.
The main columns found are 'Aircraft registration/tail number/N number','Date of Occurence','City','State','Region','Description/Remark'.

The first phase was proven successful as it showed the apprpriate results. The merged dataset is obtained.

It also proves that it is time consuming and half of the data science is completed during the data-preprocessing phase.

The modelling part is heavily implemented using the NLP i.e. Natural Language Processing techniques. It is mainly focused on the 'Description/Remarks' column.
The Latent Dirichlet Allocation (LDA) method is method used for topic modelling. The optimal number of topics are found to be 8 using the coherence factor.In the further steps, we have also found the
dominant categories from the clusters of the topics.Lastly, Naive bayes and random forest is implemented to check the accuracy of the model. It showed us some good results. 
Now, if we give a statement such as "Failure due to strike" it can automatically categorize into "Wind and hinge damage".


The dominant categories found are - 

 {0: 'Landing Issue',1: 'Accessible Area Damage',2: 'Maintenance Issue',3: 'Aircraft general Issue',4: 'Wings Damaged',5: 'Flight issue',6: 'Engine related issues',7: 'Emergency cases'}




