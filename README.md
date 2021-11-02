# Example manuscripts

This repository contains examples of fully reproducible APA manuscripts. Slides with accompanying explanations can be found [here](https://shilaan-apa.netlify.app) (note that the slides may take a minute to load). To work with the examples provided in this repository, follow the steps below.  

## 1. Installations

- Install [`R`](https://cran.r-project.org/mirrors.html)
- Install [`RStudio`](https://www.rstudio.com/products/rstudio/download/)
- Install the `RMarkdown` package  
- Install LaTeX (e.g., `TinyTex`)  

After you've installed R and RStudio, open RStudio and copy the following lines of code (one by one) into the `Console` tab to install RMarkdown and TinyTex: 

`install.packages("rmarkdown")`  
`install.packages("tinytex")`   
`tinytex::install_tinytex()`   

## 2. Clone the contents of this repository

- In `RStudio`, navigate to `File > New Project > Create Project from Version Control > Git`.  
- Under Repository URL, paste the following link: `https://github.com/shilaan/example-manuscripts.git`. 
- Click the `Browse...` button to choose a location for saving the project. 

## 3. Explore the contents of this repository 

After you've successfully cloned this repository, you will have access to a `markdown_basics` folder that includes an Rmd (`markdown_basics.Rmd`) with an overview of some formatting basics in RMarkdown and a recap of some of the aspects discussed in the [reproducible manuscript slides](https://shilaan-apa.netlify.app).  

In addition, you will have access to three subfolders with example manuscripts: `example_1`, `example_2`, and `example_3`. These examples range from most complex and detailed to least complex and detailed. `example_1`, for example, includes functions to (1) analyze data and display inline results, (2) generate and display figures, and (3) generate and display tables. `example_3` is a brief commentary that does not include any data analysis, figures, or tables. You may wish to start there if you don't have much exposure to RMarkdown yet.  

Within each folder, you will find an RMarkdown document named `manuscript.Rmd`. This is the core document that includes all the writing and code to generate the resulting fully formatted and reproducible APA manuscript named `manuscript.docx`.  

To generate this manuscript, all you need to do is open `manuscript.Rmd` and click on the `Knit` button in the RStudio toolbar. You can also use the Menu to navigate to `File > Knit` or use a shortcut: `Control + Shift + K` on Windows/Linux, or `Command + Shift + K` on OS X.  

Note that you may have to install certain R packages before you can successfully knit these documents. Here are the lines of code that you can paste into your console to do so: 

### R package installations
```
#install CRAN packages  
install.packages(c(
  "broom",
  "devtools",
  "glue",
  "here",
  "rpact",
  "rvsg",
  "tidyverse"
))

#install packages from GitHub  
devtools::install_github(c(
  "crsh/papaja@devel",
  "crsh/citr",
  "jorvlan/raincloudplots",
  "mitchelloharawild/icons"
))
```
