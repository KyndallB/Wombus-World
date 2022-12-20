# Wombus-World
<p align="center">
 <header>
   <h2>Concept:</h2>
 </header>
 </p>

   A popular Artificial Intelligence exercise is the Wumpus World; it is inspired by the video game: "Hunt the Wumpus" invented by Gregory Yob in 1973. Wumpus World serves as an introduction to knowledge-based agents and knowledge representation. In the scenario, the agent is trying to navigate a series of rooms to reach gold, while not falling into any pits or being eaten by Wombi (the plural version of Wumpus).
  
   After millions of years of evolution, the Wumpus have evolved into the far superior Wombus. These Wombi are extremely data-oriented creatures and keep track of their skills and preferences in a way that far exceeds the accuracy of traditional resumes. After sensing a great opportunity at Nelnet, the Wombus have flocked to Nelnet's careers website and used their actuators to apply for jobs across all the of Nelnet's industries. Subsequently, recruiting is overwhelmed – Nelnet simply cannot process the volume of requests and need help screening the candidates. Recruiting has sent over the spreadsheet that one of their interns prepared of all current candidates as well as a historic record of previous candidates and their most recent performance score.
  
   Unfortunately, the intern also spilled their iced mocha all over their workstation before sending us the data files. This caused the files to become corrupt. The data is still accurate, so assume no noise was added to the data set. However, some data was lost.
  
<p align="center">
<header>
                         <h3><a href="https://www.javatpoint.com/the-wumpus-world-in-artificial-intelligence">The Wumpus World Properties:</a></h3>
</header>
</p>
 
 
<p align="center">

| Properties |   | 
| Partially observable:| The Wumpus world is partially observable because the agent can only perceive the close environment such as an adjacent room.  |   
| Deterministic: | It is deterministic, as the result and outcome of the world are already known. | 
| Sequential: | The order is important, so it is sequential. | 
| Static: | It is static as Wumpus and Pits are not moving. | 
| Discrete:  | The environment is discrete. | 
| One agent: | The environment is a single agent as we have one agent only and Wumpus is not considered as an agent. | 

</p>


<p align="center">
<img width="500" src="https://repository-images.githubusercontent.com/254698189/4d035600-0afd-11eb-8052-a3f9a9d74041" alt="Wumpus World Pits and Rewards">
</p>
  
  
 <p align="center">
 <header>
 h3>Analysis & Methodology</h3>
 </header>
 </p>
 
 <p align="center">
• Shapiro-Wilk Testing was used to investigate the original datasets' distributions– both were normal. 

• The regression model was built by cross-validation in Python using train/test (70/30) subsets of data.
 
• Employee scores were used to predict and calculate candidate scores via regression analysis.

• The regression equation was used to create a new score variable for employees called "predicted score"; the predicted and original scores were compared via MSE.

• The candidate and employee descriptive statistics were compared for similarity using T-test for unequal variances. 

</p>

<p align="center">
 <img width="438" alt="image" src="https://user-images.githubusercontent.com/110564772/208702400-f7119199-13d0-4ed3-beb8-cd482ec55b07.png">
(Find a more in-depth analysis in the "Battling Bots" pdf file!)
</p> 
  
<p align="center">
 <header>
<h3>Resources:</h3>
 </header>
 </p>
 

The resources folder contains resources (csv files and instructions) used to execute analysis and produced from data transformation. 

<p align="center">

There were 2 orginal CSV files– both corrupted:

| Resources |   | 
| Original (Corrupted) Files: | wombi_candidates.csv; wombi_employees.csv |   
| Dataset Used for Regression: | employees.csv | 
| Datset used for Screening: | recruits.csv (contains imputed data for missing values and regression calclculated score) | 
| Screened Dataset: | top100.csv (top 100 candidates based on calculated/predicted score) | 
| Dataset Used for Comparison:  | emp100.csv (top 100 employees according to provided employee scores) | 

</p>


<p align="center">
 <header>
 <h3>Scripts:</h3>
 </header>
 </p>
 
The script folder contains Jupyter Notebook scripts used to perform data transformation in Python and load the transformed data into SQL for easy reference. 

| Scripts |   | 
| Analysis Based on Imputation: | wombi_candidates.csv; (*less* accurate model; ~38% accuracy; MSE= 9.3671) |   
| Analysis Without Imputation: | NonImputation Model.ipynb (*more* accurate model; ~66% accuracy; MSE= 3.2987)| 
