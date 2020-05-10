# Programming-related notes

Programming tips and tricks noted around Internet. These notes are not intended to be comprehensive.

# Table of content

* [Cheatsheets](#Cheatsheets)
* [Pipelines](#pipelines)
* [R](#r)
  * [R packages](#r-packages)
  * [Imputation](#imputation)
  * [Visualization](#visualization)
  * [Dimensionality reduction](#dimensionality-reduction)
  * [Genomics](#genomics)
  * [HowTo](#howto)
  * [Misc](#misc)
  * [R questions](#r-questions)
* [Python](#python)
* [Shell](#shell)
* [Cloud computing](#cloud-computing)
* [Miscellaneous](#miscellaneous)

## Cheatsheets

- RStudio Cheat Sheets, https://www.rstudio.com/resources/cheatsheets/
- A selection of printable, one-page cheatsheets, generated from Markdown using Pandoc & LaTeX, https://github.com/kickstartcoding/cheatsheets
- A CheatSheet for Parallel Computation in R, https://github.com/ardeeshany/Parallel_Computing

## Pipelines

- `nf-core` - a framework for Nextflow (https://www.nextflow.io/) -based pipeline creation, community-driven. Integrated with Conda, Docker, Biocontainers. Scalable to a cloud level. Pipeline assemblers: Flowcraft (https://github.com/assemblerflow/flowcraft), Pipeliner (https://github.com/montilab/pipeliner).The nf-core hub with all pipelines:https://nf-co.re/. nf-core code:https://github.com/nf-core/. Alternatives: Snakemake
    - Ewels, Philip, Alexander Peltzer, Sven Fillinger, Johannes Alneberg, Harshil Patel, Andreas Wilm, Maxime Garcia, Paolo Di Tommaso, and Sven Nahnsen. “Nf-Core: Community Curated Bioinformatics Pipelines.” Preprint. Bioinformatics, April 16, 2019. https://doi.org/10.1101/610741.

## R

### R packages

- Develop Bioconductor packages with docker container, https://divingintogeneticsandgenomics.rbind.io/post/develop-bioconductor-packages-with-docker-container/
- Steps to contribute packages to Bioconductor https://github.com/Bioconductor/Contributions
- Docker Images which include a complete installation of all software needed to build all Bioconductor packages. https://github.com/Bioconductor/bioconductor_full
- Package Building: How `DESCRIPTION`, `NAMESPACE`, `roxygen`, and `devtools::document` work together. http://laderast.github.io/2019/02/12/package-building-description-namespace/
- Automate testing of your R package using Travis CI, Codecov, and testthat. https://jef.works/blog/2019/02/17/automate-testing-of-your-R-package/
- Advice about good practices when building R packages. Advice includes functions and syntax to avoid, package structure, code complexity, code formatting, etc. https://github.com/MangoTheCat/goodpractice
- `BiocPkgTools` - R package for queueing Bioconductor package statistics, downloads, dependencies, visualization as graphs.https://bioconductor.org/packages/release/bioc/html/BiocPkgTools.html
    - Su, Shian, Vincent J. Carey, Lori Shepherd, Matthew Ritchie, Martin T. Morgan, and Sean Davis. “BiocPkgTools: Toolkit for Mining the Bioconductor Package Ecosystem.” F1000Research 8 (May 29, 2019): 752. https://doi.org/10.12688/f1000research.19410.1.
- `pkgdown` is designed to make it quick and easy to build a website for your package. https://pkgdown.r-lib.org/

**Add to README.md**

- Cross-reference the package repository under your account to the one under the `dozmorovlab` account. Like: "The developmental version is available at `your GitHub repository`, the stable version is available at `dozmorovlab GitHub repository`"
- Add BibTex citation and direct link to the paper/preprint, if relevant. [Example](https://github.com/luoyunan/DTINet)
- Add contact information. Protect e-mails against scraping, like "zengjy321[at]tsinghua[dot]edu[dot]cn" [Example](https://github.com/luoyunan/DTINet)

**Examples of well-structured software packages**

1. https://github.com/neurodata-papers/MGC
2. https://github.com/neurodata-papers/LOL
3. https://www.nature.com/nbt/journal/v34/n6/abs/nbt.3569.html#supplementary-information
4. https://www.nature.com/nature/journal/v548/n7669/full/nature23463.html#extended-data, https://github.com/yasharhezaveh/Ensai
5. https://www.nature.com/nbt/journal/v34/n11/full/nbt.3685.html#supplementary-information, https://github.com/IFIproteomics/LFQbench

### Imputation

- Missing values imputation with missMDA. Missing values imputation with missMDA
- `imputeTS` - Time Series Missing Value Imputation in R. https://journal.r-project.org/archive/2017/RJ-2017-009/index.html
- `mice` - Multivariate Imputation by Chained Equations. https://cran.r-project.org/web/packages/mice/index.html
- `missForest` - Nonparametric Missing Value Imputation using Random Forest. https://cran.r-project.org/web/packages/missForest/index.html

### Visualization

- `circlize` - Circular Visualization in R, https://cran.r-project.org/web/packages/circlize/index.html, documentation, http://zuguang.de/circlize_book/book/index.html\
- `UpSetR` - stretched and aligned venn diagram. https://www.bioconductor.org/help/course-materials/2017/BioC2017/Day1/InvitedSpeakers/relaxation-techniques-upset-data-scientist.pdf
- `visNetwork` - visNetwork is a R package for network visualization, using vis.js javascript library. https://cran.r-project.org/web/packages/visNetwork/vignettes/Introduction-to-visNetwork.html
- `DiagrammeR` - Graph and network visualization using tabular data in R. https://github.com/rich-iannone/DiagrammeR
- `autoplot` - PCA plotting. https://cran.r-project.org/web/packages/ggfortify/vignettes/plot_pca.html
- `ggord` - PCA and other dim reduction methods plotting with ellipses. https://github.com/fawda123/ggord
- `PCAtools` - set of tools performing common PCA-related tasks, by Kevin Blighe and Aaron Lun. https://github.com/kevinblighe/PCAtools, https://bioconductor.org/packages/release/bioc/html/PCAtools.html


### Dimensionality reduction

- `GLM-PCA` - multinomial distribution-based analysis methods for UMI counts in scRNA-seq data. Details of scRNA-seq data properties, analysis steps. https://github.com/willtownes/scrna2019,https://github.com/willtownes/glmpca,  https://cran.r-project.org/web/packages/glmpca/index.html
    - Townes, F. William, Stephanie C. Hicks, Martin J. Aryee, and Rafael A. Irizarry. “Feature Selection and Dimension Reduction for Single Cell RNA-Seq Based on a Multinomial Model.” BioRxiv, March 11, 2019. https://doi.org/10.1101/574574.

- PCA course using FactoMineR. https://francoishusson.wordpress.com/2017/07/13/course-on-pca-with-factominer/
- Multiple Factor Analysis to analyse several data tables. https://francoishusson.wordpress.com/2017/07/18/multiple-factor-analysis-to-analyse-several-data-tables/
- Correspondence Analysis with FactoMineR. https://francoishusson.wordpress.com/2017/07/13/correspondence-analysis-with-factominer/
- Multiple Correspondence Analysis with FactoMineR. https://francoishusson.wordpress.com/2017/07/18/multiple-correspondence-analysis-with-factominer/
- PCA, https://amunategui.github.io/high-demensions-pca/. caret::nearZeroVariance

### Genomics

- Lightweight Iterative Gene set Enrichment in R https://CRAN.R-project.org/package=liger, https://github.com/JEFworks/liger


### HowTo

- How to Create a Bar Chart Race in R - Mapping United States City Population 1790-2010. https://michaeltoth.me/how-to-create-a-bar-chart-race-in-r-mapping-united-states-city-population-1790-2010.html

- Convert continuous to categorical value

````
data(iris)
vari <- iris$Sepal.Length
nb.clusters <- 3
breaks <- quantile(vari, seq(0,1,1/nb.clusters))
Xqual <- cut(vari,breaks, include.lowest=TRUE)
summary(Xqual)
````

- Barplot with StdErr using standard R graphics

````
dat = agridat::lasrosas.corn
means.nf = tapply(dat$yield, INDEX=dat$nf, FUN=mean)  
StdErr.nf = tapply(dat$yield, INDEX=dat$nf, FUN= std.error)  
BP = barplot(means.nf, ylim=c(0,max(means.nf)+10))  
segments(BP, means.nf - (2*StdErr.nf), BP, means.nf + (2*StdErr.nf), lwd = 1.5)  
arrows(BP, means.nf - (2*StdErr.nf), BP,  means.nf + (2*StdErr.nf), lwd = 1.5, angle = 90,  code = 3, length = 0.05)  
````

- HDF5Array
````
library(HDF5Array)
a0 <- array(runif(15000000), dim=c(10000, 300, 5))
A0 <- as(a0, "HDF5Array")  
library(pryr) 
object_size(A0)
#> 1.94 kB
object_size(a0)
#> 120 MB #rstats
````

- Convert a vector to normally distributed one
````
interactions <- log2(interactions) # If highly right-skewed, log2-transform beforehand
# Inverse normal conversion
interactions <- sapply(interactions, function(x) {
  rank <- rank(x, na.last = "keep")
  P <- (rank - 0.5) / length(x[ !is.na(x)] )
  x <- qnorm(P)
})
````

### Misc

- Rcpp for machine learning notes, https://github.com/bearloga/learning-rcpp
- Simple Gantt charts in R with ggplot2 … and Microsoft Excel, https://www.molecularecologist.com/2019/01/simple-gantt-charts-in-r-with-ggplot2-and-the-tidyverse/
- `disk.frame` - blog post about disk.frame usage, https://www.brodrigues.co/blog/2019-09-03-disk_frame/
- How to make a minimal reproducible example, https://stackoverflow.com/questions/5963269/how-to-make-a-great-r-reproducible-example/5963610#5963610
- Multinomial logistic regression, https://amunategui.github.io/multinomial-neuralnetworks-walkthrough/
- `pcor` - Partial and Semi-Partial (Part) Correlation, https://cran.r-project.org/web/packages/ppcor/index.html
- `corpcor` - Efficient Estimation of Covariance and (Partial) Correlation, https://cran.r-project.org/web/packages/corpcor/index.html
- "The YAML Fieldguide", http://ymlthis.r-lib.org/articles/yaml-fieldguide.html

### R questions

- Why vcd package is used? vcd package provides different methods for visualizing multivariate categorical data.
- What is iPlots? It is a package which provide bar plots, mosaic plots, box plots, parallel plots, scatter plots and histograms.
- What is fitdistr() function? It is used to provide the maximum likelihood fitting of univariate distributions. It is defined under the MASS package.
- Define loglm() function. Loglm() function is used to create log-linear models.
- How to create scatterplot matrices? Pair() or splom() function is used for create scatterplot matrices.
- Define leaps(). It is used to perform the all-subsets regression and it is defined under the leaps package.
- Define cluster.stats(). It is define in fpc package which provide a method for comparing the similarity of two clusters solution using different validation criteria.

## Python

- Rule, Adam, Amanda Birmingham, Cristal Zuniga, Ilkay Altintas, Shih-Cheng Huang, Rob Knight, Niema Moshiri, et al. “Ten Simple Rules for Writing and Sharing Computational Analyses in Jupyter Notebooks.” PLoS Computational Biology 15, no. 7 (July 2019): e1007007. https://doi.org/10.1371/journal.pcbi.1007007. - Jupyter notebook practices. ipywidgets, watermark, papermill, nbviewer, binder. Notebook examples, https://github.com/jupyter-guide/ten-rules-jupyter, Guide for Reproducible Research and Data Science in Jupyter Notebooks, https://github.com/jupyter-guide/jupyter-guide

- Matplotlib 3.1 cheat sheet, https://github.com/rougier/matplotlib-cheatsheet

- Cleaning & Modifying A Dataframe – Python, https://datascienceplus.com/cleaning-modifying-a-dataframe-python/

- An Effective Python Environment: Making Yourself at Home. https://realpython.com/effective-python-environment/

- How to Think Like a Computer Scientist: Interactive Edition. Learning Python programming from ground up. https://runestone.academy/runestone/books/published/thinkcspy/index.html

## Shell

- `nfiletypes` function to tell the number of files of each extension type in the current directory ([Source](https://twitter.com/strnr/status/1159503398716227584?s=03)): `nfiletypes () { find . -maxdepth 1 -type f | sed 's/.*\.//' | sort | uniq -c | sed 's/^ *//g' | sed 's/ /\t/g'; }`

## Cloud computing

- cyverse tutorial links, https://github.com/crazyhottommy/cyverse_resource

## Miscellaneous

- `containerit` - an R package to create a Docker file from R session. Similar functionality provided by `dockerfiler`, `liftr`, `automagic`. https://github.com/o2r-project/containerit
    - Nüst, Daniel, and Matthias Hinz. “Containerit: Generating Dockerfiles for Reproducible Research with R.” Journal of Open Source Software 4, no. 40 (August 21, 2019): 1603. https://doi.org/10.21105/joss.01603.

- [C++ resources, part of the End-to-End Machine Learning library](https://brohrer.github.io/cpp_resources.html)

- [Intermediate C/C++ programming](http://www.langmead-lab.org/teaching-materials/#intermediate) - lecture slides by Ben Langmead
