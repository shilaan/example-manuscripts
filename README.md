# Example manuscripts

This repository contains examples of fully reproducible APA manuscripts. Slides with accompanying explanations can be found [here](https://shilaan-apa.netlify.app) (they may take a minute to load). To work with the examples provided in this repository, complete the following steps: 

## 1. Installations

- Install [`R`](https://cran.r-project.org/mirrors.html)
- Install [`RStudio`](https://www.rstudio.com/products/rstudio/download/)
- Install the `RMarkdown` package  
- Install LaTeX (e.g., `TinyTex`)  

After you've installed R and RStudio, open RStudio and copy the following lines of code into the `Console` tab (one by one) to install RMarkdown and TinyTex: 

`install.packages("rmarkdown")`  
`install.packages("tinytex")`   
`tinytex::install_tinytex()`   

## 2. Clone the contents of this repository

- In `RStudio`, navigate to `File > New Project > Create Project from Version Control > Git`.  
- Under Repository URL, paste the following link: `https://github.com/shilaan/example-manuscripts.git`. 
- Click the `Browse...` button to choose a location for saving the project. 

## 3. Explore the contents of this repository 

After you've successfully cloned this repository, you will have access to three subfolders, called `example_1`, `example_2`, and `example_3`. These examples range from most complex and detailed to least complex and detailed. The first example, for example, includes functions to (1) analyze data and display inline results, (2) generate and display figures, and (3) generate and display tables. The third example is a commentary manuscript that does not include any data analysis, figures, or tables. You may wish to start there if you don't have much exposure to RMarkdown yet. 

Within each folder, you will find an RMarkdown document named `manuscript.Rmd`. This is the core document that includes all the writing and code to generate the resulting fully formatted and reproducible APA manuscript named `manuscript.docx`.  

To generate this manuscript, all you need to do is open `manuscript.Rmd` and click on the `Knit` button in the RStudio toolbar. You can also use the Menu to navigate to `File > Knit` or use a shortcut: `Control + Shift + K` on Windows/Linux, or `Command + Shift + K` on OS X.  

Note that you may have to install certain R packages before you can successfully knit these documents. Here are the lines of code that you can paste into your console (one by one) to do so: 

### R package installations
```
#install CRAN packages  
install.packages("broom")  
install.packages("glue")  
install.packages("here")  
install.packages("rpact")  
install.packages("rsvg")  
install.packages("tidyverse")  

#install packages from GitHub  
install.packages("devtools")  
devtools::install_github("crsh/papaja@devel")  
devtools::install_github("crsh/citr")   
devtools::install_github('jorvlan/raincloudplots')  
devtools::install_github("mitchelloharawild/icons")  
```
