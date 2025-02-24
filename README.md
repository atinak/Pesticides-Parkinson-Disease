# *Under DEvelopment*

# Pesticides-Parkinson-Disease
This project aims to investigate the potential relationship between Parkinson's disease prevalence and pesticide sales in France. 
It does this by merging two datasets:


Parkinson's Disease Data: Contains the prevalence of Parkinson's disease across different regions and departments in France, broken down by year. Data : https://www.data.gouv.fr/fr/datasets/pathologies-effectif-de-patients-par-pathologie-sexe-classe-dage-et-territoire-departement-region/#/resources

Pesticide Sales Data: Contains the quantities of various pesticide active substances sold in each department of France, also broken down by year. Data: https://www.data.gouv.fr/fr/datasets/ventes-de-pesticides-par-departement/

The core of the project is a Python class (DataMerger) that performs the following key tasks:

Data Loading and Cleaning: Loads the data from CSV files, handles special cases like Corsican department codes (2A, 2B), converts data to appropriate types, and deals with potential missing values. It uses glob to efficiently handle multiple pesticide data files, organized by year.

Data Merging: Merges the Parkinson's disease data with the pesticide sales data based on year and department.

Data Transformation: Reshapes the data using a pivot table to create a format suitable for analysis, where each pesticide substance becomes a separate column.

Correlation Analysis: Calculates the correlation between Parkinson's disease prevalence and the quantities of each pesticide sold.

Data Visualization: Provides basic visualizations (histograms, time series plots, correlation heatmaps) to explore the data and potential relationships.

The project is designed to be robust, handling potential errors and variations in the data files. The ultimate goal is to provide a tool for preliminary investigation into whether there's a statistical association between pesticide exposure (as measured by sales) and Parkinson's disease prevalence, setting the stage for further, more in-depth epidemiological study. The project does not prove causation, but it can identify potential correlations that warrant further investigation.
