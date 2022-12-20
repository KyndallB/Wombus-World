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
                           <a href="https://www.javatpoint.com/the-wumpus-world-in-artificial-intelligence">The Wumpus World Properties:</a>
</p>
  
• Partially observable: The Wumpus world is partially observable because the agent can only perceive the close environment such as an adjacent room.

• Deterministic: It is deterministic, as the result and outcome of the world are already known.

• Sequential: The order is important, so it is sequential.

• Static: It is static as Wumpus and Pits are not moving.

• Discrete: The environment is discrete.

• One agent: The environment is a single agent as we have one agent only and Wumpus is not considered as an agent.

<p align="center">
<img width="500" src="https://repository-images.githubusercontent.com/254698189/4d035600-0afd-11eb-8052-a3f9a9d74041" alt="Wumpus World Pits and Rewards">
</p>
  
  
<p align="center">
                        <a href="https://www.javatpoint.com/the-wumpus-world-in-artificial-intelligence">Actuators:</a>  
</p>

<p align="center">  
• Left turn
• Right turn
• Move forward
• Grab
• Release
• Shoot
</p>

<p align="center">
<img width="500" src="https://www.massey.ac.nz/~mjjohnso/notes/59302/fig06.04.gif" alt="Wumpus World Matrix (Data Memory and Keys)">
</p>

<p align="center">
 <header>
<h3>Resources:</h3>
 </header>
 </p>

The resources folder contains resources (csv files and instructions) used to execute analysis and produced from data transformation. 

<p align="center">
There were 2 orginal CSV files– both corrupted:
 
1. wombi_candidates.csv
 
2. wombi_employees.csv
</p>

<p align="center">
There are 3 files produced from transforming and cleaning the datafiles using data imputation:
</p>
1. employees.csv (This file contains all employees with imputed data for missing values; the employees' score was used to calculate candidate scores.) 

2. recruits.csv (This file contains all candidates with imputed data for missing values; this file also contains computed candidate scores.)


3. top100.csv (This csv contains the top 100 candidates according to predicted candidate scores.)


4. emp100.csv (This csv contains the top 100 employees according to provided employee scores.)

<p align="center">
 <header>
 <h3>Scripts:</h3>
 </header>
 </p>
 
 
The script folder contains a Jupyter Notebook script used to perform data transformation in Python and load the transformed data into SQL for easy reference. 
1. The "NonImputation Model.ipynb" file is most relevant and contain the data transformations, regression analysis, and  visualizations.
2. The "Transformed_and_loaded.ipynb" file contains a regression model based on imputed data which is comparably less accurate.  
