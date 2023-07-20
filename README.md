# ESA 2023 - Introduction to the NEON Forecasting Challenge 
These materials have been developed for the 2023 Ecological Society of America meeting in Portland, Oregon as an introduction to the Ecological Forecasting Initiative and NEON Forecasting Challenge. The materials will take you through a basic workflow and will get you started on participating in the Challenge. These materials comprise of an R markdown script that generate a simple forecast of daily terrestrial fluxes of carbon and evaporation for the terrestrial NEON (National Ecological Observatory Networks) sites.

## Getting started
1. Set up your R environment (we will be using R and R Studio)
2. Download code, clone, or fork (recommended) the repository
3. Work through the example

Alternatively, you can follow along with the example via the rendered markdown document

### 1. Set up your R environment

R version 4.2 is required to run the code in this workshop. You should also check that your Rtools is up to date and compatible with R 4.2, see (https://cran.r-project.org/bin/windows/Rtools/rtools42/rtools.html). 

The following packages need to be installed using the following code.

```{r}
install.packages('remotes')
install.packages('tidyverse') # collection of R packages for data manipulation, analysis, and visualisation
install.packages('lubridate') # working with dates and times
remotes::install_github('eco4cast/neon4cast') # package from NEON4cast challenge organisers to assist with forecast building and submission
```

Make sure to restart your R session after installing any new packages!

### 2. Fork or clone the Github repository or download the code
There are 3 options for getting the code locally so that you can run it, depending on your experience with Github/Git you can do one of the following 

1. _Fork_ the repository to your Github and then clone the repository from your Github repository to a local RStudio project. This will allow you to modify the scripts and push it back to your Github. 

- Find the fork button in the top right of the webpage --> Create Fork. This will generate a copy of this repository in your Github.
- Then use the <> Code button to copy the HTTPS link (from you Github!). 
- In RStudio, go to New Project --> Version Control --> Git. 
- Paste the HTTPS link in the Repository URL space, and choose a suitable location for your local repository --> Create Project. 
- Open the .Rmd file

2. _Clone_ the workshop repository to a local RStudio project. Your local workspace will be set up and you can commit changes locally but they won't be pushed back to the Github repository.
- Find the fork button in the top left of the webpage --> Create Fork. 
- Then use the <> Code button to copy the HTTPS link.
- In RStudio go to New Project --> Version Control --> Git. 
- Paste the HTTPS link in the Repository URL space, and choose a suitable location for your local repository --> Create Project. 
- Open the .Rmd file

3. _Download_ the zip file of the repository code. You can save changes (without version control) locally.
- Find the <> Code button --> Download ZIP. 
- Unzip this to a location on your PC and open the `ESA2023_neon4cast_workshop.Rproj` file in RStudio. 

More information on forking and cloning in R can be found at [happygitwithr](https://happygitwithr.com/fork-and-clone.html), a great resource to get you started using version control with RStudio. 

### 3. Work through the example
Step through the code chunks to take you through a simple forecasting workflow and submit your first real-time forecast to the Challenge!
More information on the Challenge can be found [here](https://projects.ecoforecast.org/neon4cast-docs/)