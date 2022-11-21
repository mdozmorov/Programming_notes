# Programming-related notes

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs) [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)

Programming learning and data analysis resources. Please, [contribute and get in touch](CONTRIBUTING.md)! See [MDmisc notes](https://github.com/mdozmorov/MDmisc_notes) for other programming and genomics-related notes.

# Table of content

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [Awesome](#awesome)
- [Cheatsheets](#cheatsheets)
- [Command line](#command-line)
  - [Courses](#courses)
- [Code best practices](#code-best-practices)
- [Docker](#docker)
  - [Kubernetes](#kubernetes)
- [Cloud](#cloud)
  - [GCP](#gcp)
  - [AWS](#aws)
- [Git](#git)
- [Text](#text)
  - [Text mining](#text-mining)
- [SQL](#sql)
- [Workflows](#workflows)
  - [Makefiles](#makefiles)
  - [Snakemake](#snakemake)
  - [WDL](#wdl)
  - [Nextflow](#nextflow)
- [Web](#web)
- [Miscellaneous](#miscellaneous)
  - [Other programming languages](#other-programming-languages)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## Awesome

- [every-programmer-should-know](https://github.com/mr-mig/every-programmer-should-know) - A collection of (mostly) technical things every software developer should know

- [Learn any language X in Y minutes](https://github.com/adambard/learnxinyminutes-docs)

- [List of Data Science Cheatsheets to rule the world](https://github.com/FavioVazquez/ds-cheatsheets), PDFs covering all programming languages, machine, deep learning

- [Very large collection of free courses for all programming languages](https://github.com/vhf/free-programming-books/blob/master/free-courses-en.md), [interactive tutorials](https://github.com/vhf/free-programming-books/blob/master/free-programming-interactive-tutorials-en.md), [podcasts and screencasts](https://github.com/vhf/free-programming-books/blob/master/free-podcasts-screencasts-en.md), [books](https://github.com/vhf/free-programming-books/blob/master/free-programming-books.md). And [more, translated in other languages](https://github.com/vhf/free-programming-books)

- [awesome-javascript-learning](https://github.com/micromata/awesome-javascript-learning) - A (not so) tiny list limited to the best JavaScript Learning Resources

- [awesome-cpp](https://github.com/fffaraz/awesome-cpp) - A curated list of awesome C++ (or C) frameworks, libraries, resources, and shiny things.

- [awesome-go](https://github.com/avelino/awesome-go) - A curated list of awesome Go frameworks, libraries and software, https://awesome-go.com/

- [awesome-kubernetes](https://github.com/ramitsurana/awesome-kubernetes) - A curated list for awesome kubernetes resources. Rendered [GitBook](https://ramitsurana.github.io/awesome-kubernetes/)

- [awesome-nextflow](https://github.com/nextflow-io/awesome-nextflow) - A curated list of nextflow based pipelines, presentations, videos, tutorials.

- [awesome-pipeline](https://github.com/pditommaso/awesome-pipeline) - A curated list of awesome pipeline toolkits inspired by Awesome Sysadmin

- [awesome-readme](https://github.com/matiassingers/awesome-readme) - A curated list of awesome READMEs. Elements in beautiful READMEs include, but are not limited to: images, screenshots, GIFs, text formatting, etc.

- [awesome-workflow-engines](https://github.com/meirwah/awesome-workflow-engines) - A curated list of awesome open source workflow engines

- [useful-sed](https://github.com/adrianscheff/useful-sed) - awesome sed tips, techniques, one-liners, tutorials. By [Adrian Scheff](https://github.com/adrianscheff)

## Cheatsheets

- [awesome-reproducible-research](https://github.com/leipzig/awesome-reproducible-research) - A curated list of reproducible research case studies, projects, tutorials, and media

- [awesome-programming-books](https://github.com/majikarp/awesome-programming-books) - Awesome Programming Books

- [Best-websites-a-programmer-should-visit](https://github.com/sdmg15/Best-websites-a-programmer-should-visit) - Some useful websites for programmers

- [kickstartcoding/cheatsheets](https://github.com/kickstartcoding/cheatsheets) A selection of printable, one-page cheatsheets. HTML/CSS, Bash/Git, Python, JavaScript, Django, and more

- [quick-SQL-cheatsheet](https://github.com/enochtangg/quick-SQL-cheatsheet) - A quick reminder of all SQL queries and examples on how to use them

- [Regular expression, Unix commands, Python quick reference, SQL reference card](http://practicalcomputing.org/files/PCfB_Appendices.pdf)

## Command line

- [The 50 Most Popular Linux & Terminal Commands - Full Course for Beginners](https://youtu.be/ZtqBQ68cfJc) - a 5 hour video course

- [Bash-Oneliner](https://github.com/onceupon/Bash-Oneliner) - A collection of handy Bash One-Liners and terminal tricks for data processing and Linux system maintenance. https://github.com/onceupon/Bash-Oneliner

- [Unix/Linux command reference sheet PDF](https://cheat-sheets.s3.amazonaws.com/linux-commands-cheat-sheet-new.pdf) and [another version](https://files.fosswire.com/2007/08/fwunixref.pdf) 

- [awesome-bash](https://github.com/awesome-lists/awesome-bash) - A curated list of delightful Bash scripts and resources 

- [the-art-of-command-line](https://github.com/jlevy/the-art-of-command-line) - Master the command line, in one page. Advanced. 

- [An interactive explainer of any shell command](http://explainshell.com/) 

- [commandlinefu.com](http://www.commandlinefu.com/commands/browse) - Master the power of command-line with a list of one-liner gems

- [terminalsare.sexy](http://terminalsare.sexy) - A curated list of Terminal frameworks, plugins & resources for command-line interface (CLI) lovers. [GitHub](https://github.com/k4m4/terminals-are-sexy) 

- [ShellCheck](https://www.shellcheck.net/) finds bugs in your shell scripts

- [Awesome WSL - Windows Subsystem for Linux](https://github.com/sirredbeard/Awesome-WSL) - detailed guide for working on Linux in Windows

### Courses

- [Tools for Reproducible Research](https://uppsala.instructure.com/courses/51980/modules) - NBIS/ELIXIR course. Covers Data management, Project organisation, Git, Conda, Snakemake, Nextflow, R Markdown, Jupyter, Docker, Singularity. [GitHub](https://github.com/NBISweden/workshop-reproducible-research)

- [Introduction to Computer Science and Programming in Python](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/)

- [Survival guide for Unix newbies](http://matt.might.net/articles/basic-unix/), [Settling into Unix](http://matt.might.net/articles/settling-into-unix/), and [Shell programming with bash tutorial](http://matt.might.net/articles/bash-by-example/), by Matt Might

- [The Unix Workbench](https://seankross.com/the-unix-workbench/) by Sean Kross. From Bash basics to GitHub, cloud computing. [GitHub](https://github.com/seankross/the-unix-workbench)

- [The Unix shell](https://swcarpentry.github.io/shell-novice/), Software Carpentry

- [Data Coding 101](https://data36.com/data-coding-bash-best-practices/) – Intro To Bash. Four episodes, video

- [CSE390A](https://github.com/ldfaiztt/CSE390A) - System and Software Tools (taught by Ruth E. Anderson). Well-polished lectures and homework on Unix /Git ecosystem

- [data-science-at-the-command-line](https://www.datascienceatthecommandline.com/) - "Data Science at the Command Line" by Jeroen Janssens, [GitHub](https://github.com/jeroenjanssens/data-science-at-the-command-line)

- [Command line for data science](https://blog.robertelder.org/data-science-linux-command-line/), with examples, videos


## Code best practices

- [readme-md-generator](https://github.com/kefranabg/readme-md-generator) - CLI README generator for software packages

- [Mastering Software Development in R](https://bookdown.org/rdpeng/RProgDA/), book by Roger Peng

- [Tips for organizing projects](http://kbroman.org/steps2rr/pages/organize.html), [Organizing data in spreadsheets](http://kbroman.org/dataorg/) by Karl Broman

- [Data Organization in Spreadsheets, common mistakes](http://www.datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes/)

- [Software Carpentry reading material on software engineering and scientific computing](http://software-carpentry.org/reading/) 

- [Software development skills for data scientists](http://treycausey.com/software_dev_skills.html) by Trey Causey

- [ProjectTemplate](http://projecttemplate.net/) - an R package for advanced project management, [GitHub](https://github.com/johnmyleswhite/ProjectTemplate)

- Seemann, Torsten. “[Ten Recommendations for Creating Usable Bioinformatics Command Line Software](https://doi.org/10.1186/2047-217X-2-15).” GigaScience 2, no. 1 (December 2013)

- List, Markus, Peter Ebert, and Felipe Albrecht. “[Ten Simple Rules for Developing Usable Software in Computational Biology](https://doi.org/10.1371/journal.pcbi.1005265).” PLoS Computational Biology 13, no. 1 (January 2017)

- Taschuk, Morgan, and Greg Wilson. “[Ten Simple Rules for Making Research Software More Robust](https://doi.org/10.1371/journal.pcbi.1005412).” PLOS Computational Biology 13, no. 4 (April 13, 2017). [GitHub](https://github.com/oicr-gsi/robust-paper) 

- "Code and Data for the Social Sciences: A Practitioner’s Guide" book by Matthew Gentzkow and Jesse Shapiro, PDF. [https://web.stanford.edu/~gentzkow/research/CodeAndData.pdf](https://web.stanford.edu/~gentzkow/research/CodeAndData.pdf) 

- Wilson, Greg, D. A. Aruliah, C. Titus Brown, Neil P. Chue Hong, Matt Davis, Richard T. Guy, Steven H. D. Haddock, et al. "[Best Practices for Scientific Computing](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745) ." PLoS Biology 2014

- Noble, William Stafford. “[A Quick Guide to Organizing Computational Biology Projects](https://doi.org/10.1371/journal.pcbi.1000424).” PLoS Computational Biology 5, no. 7 (July 2009) - Computational projects organization, folder structure, command line scripts, version control


## Docker

- [Awesome-docker](https://awesome-docker.netlify.app/) - A curated list of Docker resources and projects. [GitHub](https://github.com/veggiemonk/awesome-docker)

- [An Introduction to Docker for R Users](https://colinfay.me/docker-r-reproducibility/)

-  [A comprehensive tutorial on getting started with Docker!](https://docker-curriculum.com/), by Prakhar Srivastav. [GitHub](https://github.com/prakhar1989/docker-curriculum)

- [A Docker tutorial for reproducible research](https://ropenscilabs.github.io/r-docker-tutorial/) by rOpenSci Labs

- [Docker Containers on the Desktop](https://blog.jessfraz.com/post/docker-containers-on-the-desktop/) - a collection of Docker files encapsulating various software. [GitHub](https://github.com/jessfraz/dockerfiles)

- [Docker cheat sheet](https://github.com/wsargent/docker-cheat-sheet)

- [The Docker Handbook – 2021 Edition](https://www.freecodecamp.org/news/the-docker-handbook/)

- [How Docker Can Help You Become A More Effective Data Scientist](https://towardsdatascience.com/how-docker-can-help-you-become-a-more-effective-data-scientist-7fc048ef91d5), by Hamel Husain. [Tweet by Jeremy Howard](https://twitter.com/jeremyphoward/status/1298464399527514113?s=20)

- [Docker for beginners](https://docker-curriculum.com) - Learn to build and deploy your distributed applications easily to the cloud with Docker, by Prakhar Srivastav. [Twitter](https://twitter.com/naga_rna/status/1297562599056388097?s=20)

- [Docker Jumpstart](https://github.com/odewahn/docker-jumpstart/), by Andrew Odewahn

- [Docker tutorial by Dave Tang](https://davetang.github.io/reproducible_bioinformatics/docker.html)

- [Docker Containers for Bioconductor](https://github.com/bioconductor/bioconductor_docker)

- [Docker Tutorial for Beginners - A Full DevOps Course on How to Run Applications in Containers](https://www.youtube.com/watch?v=fqMOX6JJhGo) - video course, 2 h 10 min, with interactive labs, by freeCodeCamp.org

- [Enough Docker to be Dangerous](http://seankross.com/2017/09/17/Enough-Docker-to-be-Dangerous.html) - A minimal Docker tutorial

- [Introduction to Docker](https://www.youtube.com/watch?v=Q5POuMHxW-0) - video presentation, 47 min, by Solomon Hykes

- [BioContainers](https://github.com/BioContainers/) - A community-driven project to create and manage bioinformatics software containers. [Conda, Docker/Singularity recipes](https://github.com/BioContainers/containers) to build bioinformatics software-centered containers, [specifications](https://github.com/BioContainers/specs/blob/master/container-specs.md). [mulled](https://github.com/BioContainers/mulled) and [involucro](https://github.com/involucro/involucro) helper tools. Integration with [BioConda](https://bioconda.github.io/), [Galaxy](https://galaxyproject.org/), [PhenoMeNal H2020](http://phenomenal-h2020.eu/home/). <details>
    <summary>Paper</summary>
    Veiga Leprevost, Felipe da, Björn A Grüning, Saulo Alves Aflitos, Hannes L Röst, Julian Uszkoreit, Harald Barsnes, Marc Vaudel, et al. “BioContainers: An Open-Source and Community-Driven Framework for Software Standardization.” Edited by Alfonso Valencia. Bioinformatics 33, no. 16 (August 15, 2017): 2580–82. https://doi.org/10.1093/bioinformatics/btx192.
</details>

- [Rockerverse](https://github.com/nuest/rockerverse-paper/) - Docker/containerization and R. Review of packages and applications for working with R in containers. Links to packages, examples of applications (Bioconductor, Data Science), deployment of R containers on the cloud. <details>
    <summary>Paper</summary>
     Nüst, Daniel, Dirk Eddelbuettel, Dom Bennett, Robrecht Cannoodt, Dav Clark, Gergely Daroczi, Mark Edmondson, et al. "The Rockerverse: Packages and Applications for Containerization with R" http://arxiv.org/abs/2001.10641 ArXiv:2001.10641 [Cs], January 28, 2020
</details>

- Boettiger, Carl. “[An Introduction to Docker for Reproducible Research](https://doi.org/10.1145/2723872.2723882).” ACM SIGOPS Operating Systems Review 49, no. 1 (January 20, 2015) - High-level Docker overview. Technical challenges, ways to address them (virtual machines). Docker concept of one pipeline - one image, dockerfiles, image versioning, using with RStudio, reusable modules, example commands, best practices

- Boettiger, Carl, and Dirk Eddelbuettel. “[An Introduction to Rocker: Docker Containers for R](https://journal.r-project.org/archive/2017/RJ-2017-065/index.html).” The R Journal 9, no. 2 (2017) - Rocker. Docker definitions. Command examples. Singularity. [rocker-project.org](https://www.rocker-project.org/)

### Kubernetes

- [Container Training](http://container.training/) - lecture notes and videos of various Docker, Kubernetes presentations

- [Docker Containers and Kubernetes Fundamentals – Full Hands-On Course](https://youtu.be/kTp5xUtcalw) - video course to Learn Docker containers and Kubernetes, 6h. [Website](https://kubernetesacademy.online/), [GitHub](https://github.com/K8sAcademy/Fundamentals-HandsOn)

- [Kubernetes The Hard Way On VirtualBox](https://github.com/mmumshad/kubernetes-the-hard-way) - Kubernetes The Hard Way is optimized for learning, which means taking the long route to ensure you understand each task required to bootstrap a Kubernetes cluster.

- [Kubernetes for Dummies](https://dev.to/stevenmcgown/kubernetes-for-dummies-5hmh) - introductory examples, by Steven McGown

- [future-kubernetes](https://github.com/paciorek/future-kubernetes) - instructions for setting up and using a Kubernetes cluster for running R in parallel using the future package.

- [Kubernetes Course - Full Beginners Tutorial](https://youtu.be/d6WC5n9G_sM) - 3 hour video tutorial on Kubernetes, by [Bogdan Stashchuk](https://stashchuk.com/all-courses). [GitHub](https://github.com/bstashchuk/k8s)

- [Using Kubernetes and the Future Package to Easily Parallelize R in the Cloud](https://www.r-bloggers.com/2021/04/using-kubernetes-and-the-future-package-to-easily-parallelize-r-in-the-cloud/) - how to use R on the Kubernetes cluster on Google Cloud. [Tweet](https://twitter.com/seandavis12/status/1380734816568504325?s=20)

## Cloud

- [awesome-cloudrun](https://github.com/steren/awesome-cloudrun) - A curated list of resources about all things Cloud Run

- [cloud-run-faq](https://github.com/ahmetb/cloud-run-faq) - Unofficial FAQ and everything you've been wondering about Google Cloud Run.

- [CloudBank](https://www.cloudbank.org/) - NSF-funded cloud computing for education, training, and allocation for cloud computing resources.

- [The Open Science Grid](https://opensciencegrid.org/) - A national, distributed computing partnership for data-intensive research.

- [The Cancer Genomics Cloud (CGC)](https://www.cancergenomicscloud.org/) - scientific cloud computing by Seven Bridges. Contains many public datasets (TCGA, CCLE, etc.), controlled access supported. Uses AWS. Pipelines are packaged with Docker. Execution instructions are described using Common Workflow Language (CWL). <details>
  <summary>Paper</summary>
  Lau, Jessica W., Erik Lehnert, Anurag Sethi, Raunaq Malhotra, Gaurav Kaushik, Zeynep Onder, Nick Groves-Kirkby, et al. “The Cancer Genomics Cloud: Collaborative, Reproducible, and Democratized—A New Paradigm in Large-Scale Computational Research.” Cancer Research 77, no. 21 (November 1, 2017): e3–6. https://doi.org/10.1158/0008-5472.CAN-17-0387.
</details>

- [SSH Tutorial for Linux](https://support.suso.com/supki/SSH_Tutorial_for_Linux)

## GCP

- [batch-samples](https://github.com/GoogleCloudPlatform/batch-samples) - step-by-step tutorials and code samples to learn how to use [Batch](https://cloud.google.com/batch) on Google Cloud. 

- [gcp-for-bioinformatics](https://github.com/lynnlangit/gcp-for-bioinformatics) - Google Cloud Platform (GCP) for Bioinformatics, tutorials by [Lynn Langit](https://github.com/lynnlangit). [Youtube playlist](https://www.youtube.com/playlist?list=PL4Q4HssKcxYvcixWS08UFaYIH7y4IAV0z), more cloud courses at [Lynn's profile](https://github.com/lynnlangit).

- [googleComputeEngineR](https://github.com/cloudyr/googleComputeEngineR) - An R interface to the Google Cloud Compute API, for launching virtual machines.

- [hpc-toolkit](https://github.com/GoogleCloudPlatform/hpc-toolkit) - Cloud HPC Toolkit is an open-source software offered by Google Cloud which makes it easy for customers to deploy HPC environments on Google Cloud.

## AWS

- [AWS Basics for Beginners - Full Course](https://youtu.be/ulprqHHWlng) - Video course (5h 27m) introducing topics from AWS basics to advanced cloud computing concepts. [Course code and files](https://digitalcloud.training/aws-basics-for-beginners-course-downloads/), 

- [The Open Guide to Amazon Web Services](https://github.com/open-guides/og-aws) - Amazon Web Services — a practical guide

- [Amazon Web Services](https://2016-feb-aws.readthedocs.io/) - Illustrated guide to Amazon EC2, UC Davis, Titus Brown, [Video lecture, 2 h 42 min](https://www.youtube.com/watch?v=IFdBD3YdLJc&feature=youtu.be)

- [Amazing Guide to using Amazon Web Services (AWS)](https://github.com/dwyl/learn-amazon-web-services), illustrated step-by-step tutorial

- [](https://github.com/aws/amazon-genomics-cli) - The Amazon Genomics CLI is a tool to simplify the processes of deploying the AWS infrastructure required to run genomics workflows in the cloud, to submit those workflows to run, and to monitor the logs and outputs of those workflows.

- [awesome-aws-security](https://github.com/jassics/awesome-aws-security) - Curated list of links, references, books videos, tutorials (Free or Paid), Exploit, CTFs, Hacking Practices etc. which are related to AWS Security

- [data-science-on-aws](https://github.com/data-science-on-aws/data-science-on-aws) - AI and Machine Learning with Kubeflow, Amazon EKS, and SageMaker. Code for the [Data Science on AWS](https://www.datascienceonaws.com/) book.

- [paws](https://github.com/paws-r/paws) - aws is a Package for Amazon Web Services in R. Paws provides access to the full suite of AWS services from within R. 

- Video: Amazon AWS Tutorial [#1, 22 min](https://www.youtube.com/watch?v=Xs0g_ZEv2bw), [#2, 13 min](https://www.youtube.com/watch?v=tMC4h-arGPA), [#3, 16 min](https://www.youtube.com/watch?v=z59TDrLSFx4)

## Git

- [Metrics](https://github.com/lowlighter/metrics) - An infographics generator with 30+ plugins and 200+ options to display stats about your GitHub account and render them as SVG, Markdown, PDF or JSON!

- [New to Git and GitHub? This Essential Beginners Guide is for you](https://www.analyticsvidhya.com/blog/2020/05/git-github-essential-guide-beginners/)

- [One-pager simple Git guide](https://rogerdudler.github.io/git-guide/) 

- [Resources to learn Git](https://try.github.io/) - Git handbook, cheatsheets, interactive tutorials

- [Git and GitHub guide](http://kbroman.org/github_tutorial/), by Karl Broman

- [Software Carpentry course on git](https://swcarpentry.github.io/git-novice/) 

- [Happy Git and GitHub for the useR](http://happygitwithr.com/) by Jenny Bryan

- [How to create pull requests on GitHub](https://akrabat.com/the-beginners-guide-to-contributing-to-a-github-project/) 

- Blischak, John D., Emily R. Davenport, and Greg Wilson. “[A Quick Introduction to Version Control with Git and GitHub](https://doi.org/10.1371/journal.pcbi.1004668).” Edited by Francis Ouellette. PLOS Computational Biology 12, no. 1 (January 19, 2016) - An excellent explanation of Git and GitHub. Definitions (Box 1), tutorial

- Bryan, Jennifer. “[Excuse Me, Do You Have a Moment to Talk about Version Control?](https://doi.org/10.7287/peerj.preprints.3159v2)”

- [Git and GitHub videos for beginners](http://www.dataschool.io/git-and-github-videos-for-beginners/) 

- [GitHub training videos](https://www.youtube.com/user/GitHubGuides/videos) 

- [Git and GitHub for Beginners](https://www.youtube.com/watch?v=RGOj5yH7evk) - 1-hour video course by Gwen Faraday

- [GitHub Actions for R](https://www.jimhester.com/talk/2020-rsc-github-actions/) 20 min video lecture by Jim Hester, RStudio::conf 2020

## Text

- [Curated Regular Expression Resources](https://paulvanderlaken.com/2020/04/07/curated-regular-expression-resources/), with videos

- [Learn regex the easy way](https://github.com/ziishaned/learn-regex)

- [Tutorial to sed](http://www.grymoire.com/Unix/Sed.html) by Bruce Barnett

- [Interactive Vim tutorial](http://www.openvim.com/) 

- [Vim reference card](http://web.mit.edu/merolish/Public/vi-ref.pdf) 

### Text mining

- [ralger](https://github.com/feddelegrand7/ralger) - an R package for web scraping, by M. El F. Ihaddaden. [Video](https://youtu.be/OHi6E8jegQg), 5min

- [rentrez](https://github.com/ropensci/rentrez) - Access NCIB databases, including PubMed, from R

- [PubScore](https://bioconductor.org/packages/PubScore/) - Automatic calculation of literature relevance of genes

- [Adjutant](https://github.com/amcrisan/Adjutant) - Pubmed articles analysis, word cloud, topic clustering
    - Crisan, Anamaria, Tamara Munzner, and Jennifer L Gardy. “[Adjutant: An R-Based Tool to Support Topic Discovery for Systematic and Literature Reviews](https://doi.org/10.1093/bioinformatics/bty722).” Bioinformatics, August 23, 2018. 

- [Where to get Twitter data for academic research](https://gwu-libraries.github.io/sfm-ui/posts/2017-09-14-twitter-data), blog post by Justin Littman. [Collecting, Analysing and Sharing Twitter Data](http://okfnlabs.org/blog/2018/03/08/open-data-day-tweets.html), blog post by Serah Rono

- [word2vec.r](https://word2vec.news-r.org/) - Julia's implementation of word2vec in R

- [pdftools](https://github.com/ropensci/pdftools) - Text Extraction, Rendering and Converting of PDF Documents. [Documentation](https://docs.ropensci.org/pdftools)

- [Tesseract](https://CRAN.R-project.org/package=tesseract) - Open Source OCR Engine R package

## SQL

- [sqlime](https://github.com/nalgeon/sqlime) - Online SQLite playground, for debugging and sharing SQL snippets. [Web](http://sqlime.org/)


## Workflows

- [GenPipes](https://bitbucket.org/mugqic/genpipes/src/master/) - Python pipeline framework for multi-step workflows. Over 12 pipelines for  RNA sequencing, chromatin immunoprecipitation sequencing, DNA sequencing, methylation sequencing, Hi-C, capture Hi-C, metagenomics, and Pacific Biosciences long-read assembly. Can be run via Docker. Creates executable scripts for PBS, SLURM, Batch, Daemon job schedulers. How to run: `<pipeline>.py -c myConfigurationFile -r myReadSetFile -s 1- X > Commands.txt && bash Commands.txt` where `<pipeline>` can be any of the 12 available pipelines and X is the step number desired. Commands.txt contains the commands that the system will execute. Input: FASTQ or BAM files. <details>
  <summary>Paper</summary>
  Bourgey, Mathieu, Rola Dali, Robert Eveleigh, Kuang Chung Chen, Louis Letourneau, Joel Fillon, Marc Michaud, et al. “GenPipes: An Open-Source Framework for Distributed and Scalable Genomic Analyses.” GigaScience 8, no. 6 (June 1, 2019): giz037. https://doi.org/10.1093/gigascience/giz037.
</details>

### Makefiles

- [Learn Makefiles](https://makefiletutorial.com/) With the tastiest examples, by 
[Chase Lambert](https://github.com/theicfire). [GitHub](https://github.com/theicfire/makefiletutorial)

- [Why Use Make](https://bost.ocks.org/mike/make/) blog post by Mike Bostock

- [A minimal tutorial on make](http://kbroman.org/minimal_make/) by Karl Broman

- [Learning about Makefiles](http://davetang.org/muse/2015/05/31/learning-about-makefiles/) by Dave Tang

- [Automation and Make](https://swcarpentry.github.io/make-novice/) by SoftwareCarpentry

- [Makefiles in bioinformatics](https://github.com/vsbuffalo/makefiles-in-bioinfo), one PDF lecture and four exercises

- [GNU Make - A Program for Directing Recompilation](https://www.gnu.org/software/make/manual/make.pdf) book by Stallman, Richard M., and Roland McGrath. 1991

- [List of workflow tools for R projects](https://github.com/jdblischak/r-project-workflows)

### Snakemake

- [Snakemake workflow catalog](https://snakemake.github.io/snakemake-workflow-catalog/) - a ranked list of Snakemake workflows, GitHub repositories. [Tweet](https://twitter.com/johanneskoester/status/1349806955657900034?s=20)

- [A Snakemake 'Hello world!' workflow](https://github.com/jperkel/Snakemake_example)

- [Intro to workflows for efficient automated data analysis, using snakemake](https://github.com/ctb/2019-snakemake-ucdavis), by Titus Brown, with video

- [Understanding Snakemake](https://vincebuffalo.com/blog/2020/03/04/understanding-snakemake.html) blog post by Vince Buffalo. [GitHub repo](https://github.com/vsbuffalo/snakemake-tutorial) with examples.

- [Streamlining Data-Intensive Biology With Workflow Systems](https://dib-lab.github.io/2020-workflows-paper/) - community-written review, [GitHub](https://github.com/dib-lab/2020-workflows-paper)

### WDL

- [learn-wdl](https://github.com/openwdl/learn-wdl) - Educational materials for learning WDL, by Lynn Langit

- [dg-wdl-tutorial](https://github.com/gvwilson/dg-wdl-tutorial) - Deep Genomics WDL tutorial, by Greg Wilson

- [WDL101](https://youtu.be/u5hqgNPvBlk) - 1h video workshop on using WDL on [Terra](https://terra.bio/). [Workshop material](https://drive.google.com/drive/folders/14YB0bACeaAl1XYyiyhjZJ8yyrfvlMkhv)

### Nextflow

- [nf-core](https://github.com/nf-core/) - community-curated guidelines for pipeline building using the Nextflow framework. Software bundled with pipelines using Conda, Docker/Singularity, [Bioconda](https://bioconda.github.io/), [Conda-forge](https://conda-forge.org/), [BioContainers](https://biocontainers.pro/) repositories. Software bundles (yaml environment built into Docker container), continuous integration, common structure, documentation, simplicity requirements for pipelines. Extension tools: [Flowcraft](https://github.com/assemblerflow/flowcraft) - A Nextflow pipeline assembler for genomics. [Pipeliner](https://github.com/montilab/pipeliner) - A flexible Nextflow-based framework for the definition of sequencing data processing pipelines. Similar concept - [Snakemake-workflows](https://github.com/snakemake-workflows). nf-core tools on [Bioconda](https://bioconda.github.io/recipes/nf-core/README.html) and [PyPi](https://pypi.org/project/nf-core/). [Available pipelines](https://nf-co.re/pipelines). <details>
    <summary>Paper</summary>
    Ewels, Philip A., Alexander Peltzer, Sven Fillinger, Harshil Patel, Johannes Alneberg, Andreas Wilm, Maxime Ulysse Garcia, Paolo Di Tommaso, and Sven Nahnsen. “The Nf-Core Framework for Community-Curated Bioinformatics Pipelines.” Nature Biotechnology, February 13, 2020. https://doi.org/10.1038/s41587-020-0439-x.
</details>

- [Introduction to Bioinformatics workflows with Nextflow and nf-core](https://carpentries-incubator.github.io/workflows-nextflow/aio/index.html) - The Carmentries workshop

- [nextflow-gotchas](https://github.com/Midnighter/nextflow-gotchas) - A collection of unexpected challenges and learnings with nextflow and nf-core.

- [nf-training-public](https://github.com/seqeralabs/nf-training-public) - Nextflow training material, by SequeraLabs. [Website](https://training.seqera.io/)

## Web

- [magic-of-css](https://github.com/adamschwartz/magic-of-css) - A CSS course to turn you into a magician.

- [Bootstrap CSS Framework - Full Course for Beginners](https://youtu.be/-qfEOE4vtxE) - Learn Bootstrap 5 in this full course for beginners. Bootstrap is the most popular CSS framework. It allows web developers to quickly design and customize responsive mobile-first sites. 2h46m video 

- [Bootstrap 4 Tutorials](https://www.youtube.com/playlist?list=PL4cUxeGkcC9jE_cGvLLC60C_PeF_24pvv) - playlist with short videos introducing the functionality of Bootstrap. [Bootstrap Documentation](https://getbootstrap.com/docs/4.4/getting-started/introduction/)

- [CSS Tutorial - Zero to Hero (Complete Course)](https://youtu.be/1Rs2ND1ryYc) - in depth video course by freeCodeCamp.org. [GitHub repository](https://github.com/Video-Lab/css-course-content) with the associated demo code

- [CSS Tutorial – Full Course for Beginners](https://youtu.be/OXGznpKZ_sA) - [FreeCodeCamp](https://www.freecodecamp.org/news/learn-css-in-11-hours/) 11 hours video course for frontend web developers.

- [Build a website with blogdown in R](https://erum2020.netlify.app/) presentation by Tatjana Kecojevic, [GitHub](https://github.com/TanjaKec/eRum2020)

- [JavaScript for Data Science](https://js4ds.org) - detailed instructions by Maya Gans, Toby Hodges, and Greg Wilson

- [d3graphTheory](https://mrpandey.github.io/d3graphTheory/) - Interactive webapp meant to be used as graph theory tutorials. Topics include: "Vertices and Edges", "Order and Size of a Graph", "Degree of a Vertex", "Degree Sequence of a Graph", "Graphic Sequence", "Havel-Hakimi Algorithm", "Pigeonhole Principle", "Regular Graph", "Complete Graph", "Bipartite Graph", "Complete Bipartite Graph", "Walk", "Open vs Closed Walks", "Connectivity", "Eulerian Circuit", "Eulerian Trail". [GitHub](https://github.com/mrpandey/d3graphTheory)

- [D3 in Depth](http://d3indepth.com/)

- [Datavis 2020](https://datavis.tech/datavis-2020/) - a free online course about how to conceptualize, design, and build interactive data visualizations with Web technologies. Videos, notes


## Miscellaneous

- [Ubuntu on Windows for computational biology](https://www.protocols.io/view/ubuntu-on-windows-for-computational-biology-sfuebnw) - How to install Ubuntu on Windows , by James Lloyd. [Twitter](https://twitter.com/StevenXGe/status/1297149642686242816?s=20)

- [Research computing teaching materials developed by School of Medicine Research Computing at the University of Virginia](https://github.com/uvarc/courses) - Cloud, Docker, command line, Git, Python, genomics

- The Bioconda Team, Björn Grüning, Ryan Dale, Andreas Sjödin, Brad A. Chapman, Jillian Rowe, Christopher H. Tomkins-Tinch, Renan Valieris, and Johannes Köster. “[Bioconda: Sustainable and Comprehensive Software Distribution for the Life Sciences](https://doi.org/10.1038/s41592-018-0046-7).” Nature Methods 15, no. 7 (July 2018) - Conda, Bioconda overview

- [condacolab](https://github.com/conda-incubator/condacolab) - Install Conda and friends on Google Colab

- [Diátaxis](https://diataxis.fr/) - A systematic framework for technical documentation authoring.

- [netdata.cloud](https://www.netdata.cloud) - Real-time performance monitoring, done right! Over 200 zero-configuration-supported systems, hardware, containers, and applications, from Docker/Kubernetes to databases/web servers, and more.

### Other programming languages

See [R_notes](https://github.com/mdozmorov/R_notes) and [Python_notes](https://github.com/mdozmorov/Python_notes) repositories for those languages 

- [CMake Cookbook](https://github.com/dev-cafe/cmake-cookbook) - This repository collects sources for the recipes contained in the CMake Cookbook published by Packt and authored by Radovan Bast and Roberto Di Remigio

- [Java Programming for Beginners – Full Course](https://youtu.be/A74TOX803D0) - 4h 10m video course, from Hello World to Object Oriented Programming

- [Learn C Programming with Dr. Chuck (feat. classic book by Kernighan and Ritchie)](https://youtu.be/j-_s8f5K30I) - video course, 9h38m

- [learngo](https://github.com/inancgumus/learngo) - 1000+ Hand-Crafted Go Examples, Exercises, and Quizzes

- [linguist](https://github.com/github/linguist) - This library is used on GitHub.com to detect blob languages, ignore binary or vendored files, suppress generated files in diffs, and generate language breakdown graphs.

- [How_to_learn_modern_Rust](https://github.com/joaocarvalhoopen/How_to_learn_modern_Rust) - video and text resources for learning Rust

- [project-based-learning](https://github.com/practical-tutorials/project-based-learning) - Curated list of project-based tutorials in various programming languages, general purpose, web, many more.

- [The Rust Programming Language](https://doc.rust-lang.org/book/) book, [Cookin' with Rust](https://rust-lang-nursery.github.io/rust-cookbook/intro.html) cookbook, [Why scientists are turning to Rust](https://www.nature.com/articles/d41586-020-03382-2) Nature technology feature

- [Tutorials on Topics in Julia Programming](https://github.com/johnmyleswhite/julia_tutorials) - Mastering Julia for Statistical Computing and more

- [C++ resources, part of the End-to-End Machine Learning library](https://brohrer.github.io/cpp_resources.html)

- [Intermediate C/C++ programming](http://www.langmead-lab.org/teaching-materials/#intermediate) - lecture slides by Ben Langmead

- [Rcpp for everyone](https://teuder.github.io/rcpp4everyone_en/) - Rcpp for everyone, by Masaki E. Tsuda. [GitHub](https://github.com/teuder/rcpp4everyone_en)

