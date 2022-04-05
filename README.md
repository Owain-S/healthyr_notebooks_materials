# Getting started:

Create a free RStudio Cloud account and take a copy of the HealthyR Notebooks project following this link:
https://rstudio.cloud/project/3850635

1. Create an account
2. Click on "Take a permanent copy" at https://rstudio.cloud/project/3850635
3. Click on the `01_introduction` folder in the Files pane (bottom-right), then open `01_introduction.Rmd`

## Videos

1.	Installing R
    - Windows: https://media.ed.ac.uk/media/Installing+R+for+Windows/1_rjmwhomf
    - Mac: https://media.ed.ac.uk/media/Installing+R+for+Mac/1_6ehnxok0
2.	Installing RStudio
    - Windows: https://media.ed.ac.uk/media/Installing+RStudio+for+Windows/1_vofip4cg
    - Mac: https://media.ed.ac.uk/media/Installing+RStudio+for+Mac/1_zql53iva
3.	Installing R packages: https://media.ed.ac.uk/media/Installing+R+Packages/1_2yfie5da
4.	Exploring RStudio: https://media.ed.ac.uk/media/Exploring+RStudio/1_0bdm2dxf
5.	Welcome to R: https://media.ed.ac.uk/media/Welcome+to+R/1_is6b5a1d
6.	RStudio Projects: https://media.ed.ac.uk/media/RStudio+Projects/0_06t7jmhd
7.	Importing CSV files: https://media.ed.ac.uk/media/Importing+CSV+Files/1_ntwi93hq
8.	Importing Excel files: https://media.ed.ac.uk/media/Importing+Excel+files/0_7k3z7x1a
9.	Exploring data: https://media.ed.ac.uk/media/Exploring+Data/0_0x81oy5g
10.	Preparing data: https://media.ed.ac.uk/media/Preparing+Data/0_2w3an1sj
11.	Tidying data: https://media.ed.ac.uk/media/Tidying+Data/1_6lvj81qx


All videos: https://media.ed.ac.uk/tag/tagid/healthyr

### For offline use, follow the steps below to install everything on your own computer:

## 1. R

Download and install the latest version of R from:

https://www.stats.bris.ac.uk/R/

*Mac*: `Download R for (Mac) OS X` - `R-4.1.2.pkg`

*Windows*: `Download R for Windows` - `base`


## 2. RStudio

Then download and install RStudio:

https://www.rstudio.com/products/rstudio/download/#download


## 3. R packages

### 3.1 Open RStudio and copy-paste the lines below into the Console and press Enter:

```{r}

healthyr_notebooks = c("tidyverse", "boot", "finalfit", "flexdashboard",
"gapminder", "here", "kableExtra", "knitr", "remotes",
"rmarkdown", "shiny", "survminer", "tinytex", "patchwork")
install.packages(healthyr_notebooks)

```

## 3.2 Then Restart R

## 3.3 to then run this this line (same as before, copy-paste to the Console):

```{r}

tinytex::install_tinytex()

```

If it asks you "Do you want to restart your R session", press **Yes** the first time. If it immediately asks again, press **No**.

Code to check tinyTex and Tex working as expected:

```{r, eval = FALSE}

tinytex:::is_tinytex()

#  If installed should return `TRUE`.
# Notice the triple colon, this is because it's an internal variable name.

```

### Troubleshooting

`~"TeX failed, you already have a TeX distribution...".`
If you already have LaTex installed on your computer, the `tinytex::install_tinytex()` one is not necessary and might not work.  This is fine, there is no harm in copy-pasting in anyway if you are not sure.


`WARNING: Rtools is required to build R packages, but is not currently installed.`

Some packages need a little extra help on installation. This can happen if the package developer hasn't uploaded the Windows binaries to CRAN, or if you're installing directly from GitHub. Mac's have this capability built in, whereas Windows users will have to install RTools before trying to install package again: https://cran.r-project.org/bin/windows/Rtools

## 4. Set up course materials

1. Click on `Clone or download` then `Download ZIP` (top-right of this GitHub page)
2. Unzip the folder and rename it to just healthyr (so from `healthyr_notebooks_materials-master` to `healthyr`).
3. Move this folder to where you will be keeping your R projects. Each RStudio project is in a separate folder, but you can always move them afterwards (e.g. into a new folder called R-projects).
4. Open RStudio. Click on New Project.
5. Select "Existing Directory".
6. Browse to find your `healthyr` folder, then `Create Project`.
7. Click on the `01_introduction` folder in the Files pane (bottom-right), then open `01_introduction.Rmd`.
