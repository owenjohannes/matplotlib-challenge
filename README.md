# matplotlib-challenge

## Pymaceuticals
The script reads two clinical study datasets in CSV format to generate all of the tables and figures needed for a technical report.

### Data
The CSV file 'mouse_metadata_path' is located in 'data/Mouse_metadata.csv' and contains five columns, 'MOUSE ID', 'Drug Regimen', 'Sex', 'Age_months' and 'Weight (g)'. The file's first row is a header row.
The CSV file 'study_results_path' is located in 'data/Study_results.csv' and contains four columns, 'MOUSE ID', 'Timepoint', 'Tumor Volume (mm3)' and 'Metastatic'. The file's first row is also a header row.
The script combines both datasets into a single dataset 'metadata_results_complete'.

### Code Operation
Operating the code involves running the file 'pymaceuticals.ipynb'.
The analysis will drop the duplicate mouse 'g989' to create a clean dataframe, before outputting summary statistics for the clinical study.
In order to generate a line plot of tumor volume vs. time point for a mouse treated with Capomulin, the 'mouse_id' of the mouse treated with Capomulin needs to be inputted.


### Dependencies
This program requires the matplotlib, pandas as well as scipy.stats libraries.

### Analysis
The analysis outputs these tables and figures:
    
A summary statistics table of mean, median, variance, standard deviation, and SEM of the tumor volume for each regimen.     
A bar plot showing the total number of timepoints for all mice tested for each drug regimen.     
A pie plot showing the distribution of female versus male mice.     
A box plot that shows the distrubution of the tumor volume for each treatment group ['Capomulin', 'Ramicane', 'Infubinol', 'Ceftamin']
as well as any potential outliers.     
A line plot of tumor volume vs. time point for a mouse treated with Capomulin.     
A scatter plot of average tumor volume vs. mouse weight for the Capomulin regimen as well as the regression line of the data.
        
           
           
