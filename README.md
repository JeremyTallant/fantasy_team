# Scout your Athletics Fantasy Team
## Description
If you were scouting out an athletics team, you would need to know more than just how far each person has jumped or thrown once. You want to know who is the most consistent, who fouls the least and who comes through in the clutch. And you will need to decide which aspects are most important to you so you can find the right balance.

In this R project, we will use dataframes and the `dplyr` package to find out who you should put on our team, and in doing so become the next "Moneyball" star manager of an athletics team.

We will use performance data collated from jumps and throws events in the US from 2013-2017.
## Usage
Clone this repository and open the Jupyter notebook file (`*.ipynb`) in a Jupyter environment with R kernel support. Make sure to install the required packages such as `tidyverse`. You can do this by running the following commands in a code cell within the notebook:
``` r
install.packages("tidyverse")
```
Once the packages are installed, run the code cells in the notebook to generate the plots and analyses.

If you don't have a Jupyter environment set up, you can install Jupyter Notebook and the R kernel using the following steps:

1. Install Jupyter Notebook by following the instructions on the [official Jupyter website](https://jupyter.org/install).

2. Install the R kernel for Jupyter Notebook by running the following commands in your R console:
``` r 
install.packages("IRkernel")
IRkernel::installspec()
```
After completing the installation, launch Jupyter Notebook, navigate to the folder containing the notebook file, and open it to begin running the analysis.
## Contents
1. **Athletics needs a new breed of scouts and managers:** Read in the dataset and extract the events of interest.
2. **Managers love tidy data:** Put the data in a tidy format, where each observation is the result from an individual flight.
3. **Every throw matters:** For each meet an athlete competed in, we want to know the total distance covered, the standard deviation of each athlete's successful throws and the number of successful throws.
4. **Find the clutch performers:** Use the data frame `javelin` to find the difference between the first three throws and second three throws for each athlete in each event.
5. **Pull the pieces together for a new look at the athletes:** Join the diff column from javelin to the javelin_totals data frame that contains the other summary statistics.
6. **Normalize the data to compare across stats:** Apply a function to normalize the data across aggregate statistics then compute each athlete's average for each of the normalized stats.
7. **What matters most when building your squad?:** Choose the weights for our statistics.
8. **Get to know your players:** Create a data frame `team_stats` containing your players' average statistics from the `javelin_totals` data frame. 
9. **Make your case to the front office:**
10. **Time to throw down:**

