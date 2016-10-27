# The statistical Analysis of the Inner Ear
This project used Python and python data analysis library [Pandas](http://pandas.pydata.org/)in order to parse, structure and analyse the large MRI datasets obtained during the project. 
Visualisation of the project data was achieved using a plotting library called [matplotlib](http://matplotlib.org/) and analysis was completed using the [SciPy library](https://www.scipy.org/)

## Project Description

This study looks to quantify spatial and temporal inflammation-induced changes in the capsular permeability and macrophage infiltration in guinea-pig cochlea using MRI. Modelling of such exchanges in blood and different inner ear (IE) compartments require the analysis of a substantial amount of data. 

This data has been extracted from a set of MRI which measures the propagation of a contrast agent injected into the IE. This project aims to investigate the parsing of this data and statistical analysis of these results. 

This project could provide reference data that can in future be used to quantitatively assess the treatment of ear disease in animal models and establish a platform from which such techniques can be transferred into clinical practice. 


### Prerequisities

1. **Python**
   - Successful running of this programme will require Python 2.7.12
   - You can download Python 2.7.12 following [This link ](https://www.python.org/downloads/release/python-2712/)  
   - Alternatively, you may alter the script to fit your version of Python

2. **Operating System**
  - Ubuntu 16.04 LTS 


3. **Data File Requirements**
 - Data Files must be text files (.txt)
 - Files should be labeled like this: **(no.of images)D(no.days after treatment or non-treatment)**
 - So the name should contain **a number** followed by a **D** then another **number**
 - For example: a file labeled **13D4** is an animal that has been imaged 13 times, 4 days after treatment 
 
##Running the programme using the test data
###Loading project_IE.py
1) Download the test_Project_IE folder and transfer the project_IE.py
2) Open a command line terminal in the folder containing project_IE.py
 
3) Type in python project_IE.py in the command window 
4) Once this is complete you should be greeted with the first menu 

   ```
   Welcome to Project IE
   your options are:

   1) One file
   2) Quit

   Choose your option:
   ```
   
   - If you would like to exit the programme you can type `2` otherwise keep reading the instructions 
###Loading dummy data 
1. Type `1`
 - If you enter an invalid number a message will appear saying 
   
   `The number you have entered is invalid please choose either option 1 or 2 `
   
2. Type in `10D4`
   - Your DataFrames should print now this should be followed by a message that reads: 

   ```
   Your graph has been plotted and saved
   You may choose another option now
   
   ```
3. The secondary  menu should greet you now
   ```
   What would you like to do now?
 
   1) visualisation
   2) one-way ANOVA
   3) Quit
   
   Choose your option: 
   ```

###Visualisation 
1. Type `1` for a visualization
2. A graph should automatically save in your folder called `Your Graph`
3. A new message will appear 
   ```
   Your graph has been plotted and saved.

   You may choose another option now.
   ```
4. Once this is complete you will be greeted by the secondary menu again 

### one-way ANOVA 
1. Type `2` for a one-way ANOVA
2. A message should appear saying: 
   `One-way ANOVA followed by your P value` 
3. An interpretation of your p-value should this output 
      - If it is significant (p-value = <0.05)
      
      ```
      The differences between some of the means are statistically significant
     
      Your analysis is complete.

      You may choose another option now.
      ```
      - If it is not significant 
      
      ```
      The differences between the means are not statistically significant
     
      Your analysis is complete.

      You may choose another option now.
      ```
 
 Once complete you can now exit the programme by typing `3`
