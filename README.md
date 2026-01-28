Project Title:
Environmental Drivers of Animal Species Richness in Ponds

Project Description:
This project examines how environmental conditions and pond characteristics influence animal species richness across ponds in the Madison, Wisconsin area. Using observational data collected from multiple pond types (urban, rural, and green space), the analysis explores relationships between species richness and variables such as pH, salinity, conductivity, dissolved oxygen, water temperature, and seasonality. Statistical analyses and visualizations were conducted in R and documented in a reproducible R Markdown report.

Data Description:
The dataset includes biological survey data and environmental measurements collected from 272 sampling sites across 68 ponds during the months of May–August in 2019 and 2020. Species were identified in the laboratory following field sampling using dip nets and seine nets (https://dex.edirepository.org/dex/profile/1104). Environmental variables were measured in situ using handheld water quality meters.

Key variables include:

Animal.Rich: Number of animal species observed (response variable)
Total.Rich: Total species richness at each site
Salinity, Conductivity, pH, DO.mg, Water.Temp, Chloride: Environmental predictors
Month: Sampling month (May–August)
Pond.Type: Pond classification (Urban, Rural, Green Space)
Round: Sampling round identifier
Derived variables (e.g., total non-animal richness) were created during data processing.

Methods Overview:
The data were cleaned by selecting relevant variables and removing missing values. Exploratory analyses and visualizations were used to examine seasonal and environmental trends in animal species richness. Linear regression models were applied to assess relationships between richness and individual environmental variables, followed by multiple regression models to evaluate combined effects. A linear mixed-effects model was used to account for variability among pond types. Model diagnostics were conducted to assess assumptions and model fit.

Code and File Structure:
R Markdown file (.Rmd): Contains all data processing, analysis, visualization, and interpretation
CSV file(s): Raw pond survey and environmental data
PDF output: Final rendered report with figures, tables, and results

README.txt: Project overview and data documentation

Software Requirements:

R (version 4.0 or higher recommended)
R packages: tidyverse, ggplot2, lme4, cowplot, knitr

Reproducibility:
All analyses are fully reproducible using the provided R Markdown file and dataset. Running the .Rmd file will regenerate all figures, tables, and model outputs.

Please Note:
This project was conducted to satisfy the course requirements for graduate course Environment 710: Applied Statistical Modeling for Environmental Management at Duke University. Not all code is included in this Github repository. 

Authors / Contributors:
This project was completed collaboratively by all group members, with shared contributions to data analysis, code development, and written interpretation. For this project, I developed a reproducible R-based workflow to analyze how environmental variables influence animal species richness across ponds in the Madison, Wisconsin area. I cleaned and subset the dataset, created derived variables, and used linear and mixed-effects regression models to evaluate the influence of abiotic factors, seasonality, and pond type on species richness. Results were visualized using ggplot2, model assumptions were assessed through diagnostics, and all analyses were documented in an integrated R Markdown report.

References:
Oertli, B., & Parris, K. M. (2019). Toward management of urban ponds for freshwater biodiversity. Ecosphere, 10(7).
Sax, D. F., & Gaines, S. D. (2003). Species diversity: from global decreases to local increases. Trends in Ecology & Evolution, 18, 561–566.
