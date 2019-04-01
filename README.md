# Programming-related notes

Programming tips and tricks noted around Internet. These notes are not intended to be comprehensive. They include notes about methods, packages and tools I would like to explore. For a comprehensive overview of the subject, consider [other bioinformatics resources](https://github.com/mdozmorov/blogs). Issues with suggestions and pull requests are welcome!

# Table of content

* [Cheatsheets](#Cheatsheets)
* [R packages](#r-packages)
  * [Visualization](#visualization)
  * [Dimensionality reduction](#dimensionality-reduction)
  * [HowTo](#howto)
    * [Convert continuous to categorical value](#convert-continuous-to-categorical-value)
    * [Barplot with StdErr using standard R graphics](#barplot-with-stderr-using-standard-r-graphics)
  * [Misc](#misc)
    * [R questions](#r-questions)
* [Cloud computing](#cloud-computing)

## Cheatsheets

- List of Data Science Cheatsheets to rule the world, https://github.com/FavioVazquez/ds-cheatsheets
- RStudio Cheat Sheets, https://www.rstudio.com/resources/cheatsheets/
- A selection of printable, one-page cheatsheets, generated from Markdown using Pandoc & LaTeX, https://github.com/kickstartcoding/cheatsheets
- A CheatSheet for Parallel Computation in R, https://github.com/ardeeshany/Parallel_Computing

## R packages

- Steps to contribute packages to Bioconductor https://github.com/Bioconductor/Contributions
- Package Building: How `DESCRIPTION`, `NAMESPACE`, `roxygen`, and `devtools::document` work together. http://laderast.github.io/2019/02/12/package-building-description-namespace/
- Automate testing of your R package using Travis CI, Codecov, and testthat. https://jef.works/blog/2019/02/17/automate-testing-of-your-R-package/

### Visualization

- `circlize` - Circular Visualization in R, https://cran.r-project.org/web/packages/circlize/index.html, documentation, http://zuguang.de/circlize_book/book/index.html\
- `UpSetR` - stretched and aligned venn diagram. https://www.bioconductor.org/help/course-materials/2017/BioC2017/Day1/InvitedSpeakers/relaxation-techniques-upset-data-scientist.pdf
- `visNetwork` - visNetwork is a R package for network visualization, using vis.js javascript library. https://cran.r-project.org/web/packages/visNetwork/vignettes/Introduction-to-visNetwork.html
- `DiagrammeR` - Graph and network visualization using tabular data in R. https://github.com/rich-iannone/DiagrammeR
- `autoplot` - PCA plotting. https://cran.r-project.org/web/packages/ggfortify/vignettes/plot_pca.html
- `ggord` - PCA and other dim reduction methods plotting with ellipses. https://github.com/fawda123/ggord

### Dimensionality reduction

- PCA course using FactoMineR. https://francoishusson.wordpress.com/2017/07/13/course-on-pca-with-factominer/
- Multiple Factor Analysis to analyse several data tables. https://francoishusson.wordpress.com/2017/07/18/multiple-factor-analysis-to-analyse-several-data-tables/
- Correspondence Analysis with FactoMineR. https://francoishusson.wordpress.com/2017/07/13/correspondence-analysis-with-factominer/
- Multiple Correspondence Analysis with FactoMineR. https://francoishusson.wordpress.com/2017/07/18/multiple-correspondence-analysis-with-factominer/
- Missing values imputation with missMDA. Missing values imputation with missMDA
- PCA, https://amunategui.github.io/high-demensions-pca/. caret::nearZeroVariance

### HowTo

#### Convert continuous to categorical value

````
data(iris)
vari <- iris$Sepal.Length
nb.clusters <- 3
breaks <- quantile(vari, seq(0,1,1/nb.clusters))
Xqual <- cut(vari,breaks, include.lowest=TRUE)
summary(Xqual)
````

#### Barplot with StdErr using standard R graphics

````
dat = agridat::lasrosas.corn
means.nf = tapply(dat$yield, INDEX=dat$nf, FUN=mean)  
StdErr.nf = tapply(dat$yield, INDEX=dat$nf, FUN= std.error)  
BP = barplot(means.nf, ylim=c(0,max(means.nf)+10))  
segments(BP, means.nf - (2*StdErr.nf), BP, means.nf + (2*StdErr.nf), lwd = 1.5)  
arrows(BP, means.nf - (2*StdErr.nf), BP,  means.nf + (2*StdErr.nf), lwd = 1.5, angle = 90,  code = 3, length = 0.05)  
````

### Misc

- Multinomial logistic regression, https://amunategui.github.io/multinomial-neuralnetworks-walkthrough/
- `pcor` - Partial and Semi-Partial (Part) Correlation, https://cran.r-project.org/web/packages/ppcor/index.html
- `corpcor` - Efficient Estimation of Covariance and (Partial) Correlation, https://cran.r-project.org/web/packages/corpcor/index.html
- `imputeTS` - Time Series Missing Value Imputation in R. https://journal.r-project.org/archive/2017/RJ-2017-009/index.html
- `mice` - Multivariate Imputation by Chained Equations. https://cran.r-project.org/web/packages/mice/index.html

#### R questions

- Why vcd package is used? vcd package provides different methods for visualizing multivariate categorical data.
- What is iPlots? It is a package which provide bar plots, mosaic plots, box plots, parallel plots, scatter plots and histograms.
- What is fitdistr() function? It is used to provide the maximum likelihood fitting of univariate distributions. It is defined under the MASS package.
- Define loglm() function. Loglm() function is used to create log-linear models.
- How to create scatterplot matrices? Pair() or splom() function is used for create scatterplot matrices.
- Define leaps(). It is used to perform the all-subsets regression and it is defined under the leaps package.
- Define cluster.stats(). It is define in fpc package which provide a method for comparing the similarity of two clusters solution using different validation criteria.

## Cloud computing

- cyverse tutorial links, https://github.com/crazyhottommy/cyverse_resource
