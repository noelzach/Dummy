# Coding Challenge 4

## Question 1

1.  A YAML header is …
2.  A pull request is when …

## Question 2: Coding challenge 2 in .r markdown format

Here, we will analyze mycotoxin data collected from wheat heads grown in
the greenhouse inoculated with Fusarium graminearum (Fg) with or without
fungal endophytes to protect against Fg. The experiment was performed by
inoculating the heads with Fg (positive control), Fg + 1 of 3 endophytes
(Fg + 40, Fg + 70, or Fg + 37), and the non-treated control (NTC).
Therefore, the experiment was five treatments with 6-10 technical
replicates and three experimental replicates. The authors quantified the
parts per million (ppm) of mycotoxins Deoxynivalenol (DON) and the
variant 15ADON from the wheat grain, and this is your primary response
variable. In other words, we are interested in knowing if the fungal
endophytes could reduce the concentration of DON on wheat heads. This
was done across two wheat cultivars, a winter wheat variety, Ambassador,
and a spring wheat variety, Wheaton. These data are published here:

### Question 2a - clickable link

- Noel, Z.A., Roze, L.V., Breunig, M., Trail, F. 2022. Endophytic fungi
  as promising biocontrol agent to protect wheat from Fusarium
  graminearum head blight. Plant Disease.
  <https://doi.org/10.1094/PDIS-06-21-1253-RE>
- The following github repository is associated with this paper:
  <https://github.com/noelzach/EndophyteBiocontrol>

### Load in the library you will need

``` r
library(ggplot2)
library(ggpubr)
```

### Question 2b - Read in the data using a relative file path

``` r
DON_data <- read.csv("CodingChallenge4/MycotoxinData.csv", na.strings = "na")
str(DON_data)
```

    ## 'data.frame':    375 obs. of  6 variables:
    ##  $ Treatment     : chr  "Fg" "Fg" "Fg" "Fg" ...
    ##  $ Cultivar      : chr  "Wheaton" "Wheaton" "Wheaton" "Wheaton" ...
    ##  $ BioRep        : int  2 2 2 2 2 2 2 2 2 3 ...
    ##  $ MassperSeed_mg: num  10.29 12.8 2.85 6.5 10.18 ...
    ##  $ DON           : num  107.3 32.6 416 211.9 124 ...
    ##  $ X15ADON       : num  3 0.85 3.5 3.1 4.8 3.3 6.9 2.9 2.1 0.71 ...

### Colorblind pallet needed.

``` r
cbbPalette <- c("#000000", "#E69F00", "#56B4E9", "#009E73", "#F0E442", "#0072B2", "#D55E00", "#CC79A7")
```

### Question 2c

### DON figure

### 15A DON

### Seedmass

### Combine them all togetether

## Question 3

A table of contents was created by editing the YAML header, and can be
viewed in the rendered docx or pdf document.

## Question 4

A directory was created inside my top level directory called coding
challenge 4 for my repository and I put the .md and .docx files there.

## Question 5

I edited the readme of my repository to make a clickable link to the .md
file so it was viewable on github.

## Question 6

This is a link to my GitHub <https://github.com/noelzach/Dummy>
