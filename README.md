# Applied Machine Learning I: Stroke Prediction with LM, GLM, NN and SVM

**Authors:**  Larissa Eisele, Fabian Lüthard & Yves Maillard

**Module:** Applied Machine Learning I (June 2022)

**Study Program:** Master of Science in Appplied Information & Data Science

**Supervisor:** Matteo Tanadini and Daniel Meister


## Project Structure

```
|--eisele-luethard-maillard-mpm02-stroke-prediction.pdf       # Report rendered by Bookdown 
|--data\              # Data for the analysis (CSV)
|--latex\             # Custom Title Page in Latex
|--references\        # References
  |--references.bib     # BibTeX references
  |--apa.csl            # APA 7th Edition Citation Style Language

|--eisele-luethard-maillard-mpm02-stroke-prediction.html      # Report rendered by Bookdown
```

# Installation

The following packages are required to knitr this report using bookdown.

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE, messages = FALSE)
packages <- c("dplyr","readxl", "curl", "ggplot2", "ggrepel", "maps", "plotly", "stringr", "tm", "wordcloud2", "tidyverse", "RColorBrewer", "ggwordcloud", "viridis", "bookdown", "utils", "leaps", "broom","GGally", "e1071", "caret", "mgcv", "imbalance", "MLmetrics", "neuralnet")
package.check <- lapply(packages, FUN = function(x) {
    if (!require(x, character.only = TRUE)) {
        install.packages(x, dependencies = TRUE)
        library(x, character.only = TRUE)
    }
})
```

# Rendering
In R-Studio click on the arrow on Knit then select "Knit to pdf_document2" or "Knit to pdf_html2". The following project was compiled using RStudio 2021.09.2 Build 382 and R version 4.1.2 (2021-11-01).
