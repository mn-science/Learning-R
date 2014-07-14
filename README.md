---
title: "Learning R"
author: "MPCA Stats and R Users"
date: "July 15, 2014"
output:
  html_document:
    toc: true
    theme: flatly
    highlight: tango
---

* * * *
Our own GitHub
========================================================

- [www.github/mn-stats](www.github/mn-stats)


* * * *
#Intro
>My goal is to make R more accessible to you, to help you find
>a niche or a foothold that interests you and aligns with the work
>you are doing now, and from there you will be able to launch
>yourself into learning more about the wider world of R and possibly
>making it part of your everyday routine.


>R has something for everyone. If there is something you want to do faster, or something you wish you didn't have to do twice,
>if you've ever wished you had more control over how your charts look,or think it would be useful to have your analysis process
>documented, or wishing someone could just send you an e-mail of the steps they took so you could see how they came to different
>conclusions from the same numbers. Are ou forced to cut corners due to time constraints or limit your analysis? 
>If you've ever heard someone say, let's just quality check the top 10% offenders, or we only have time to analyze the metro counties...
  
>R can help you.  


Table of Contents
---

1. What is R?
2. Point & Click
3. Tutorials
4. Internet Search
5. Manuals
6. Videos
7. Books
8. Quick Reference
9. Help

* * * *
What is R?
========================================================
- R is a <a href="http://www.r-project.org/" target="_blank">free, open-source language and environment</a>
for statistical analysis

- R is more than stats software or a free version of SAS or SPSS
  > - Documenting, GIS, Simulations, Automating, Interactive charts, Web tools

- But don't worry, it doesn't have to be
 - Easy stats tasks are still easy in R, so don't get scared away

```{r, echo=F}
AirQuality=airquality[,c(3,1)]
par(mar=c(4.2,4.2,1,1), pch=1, cex=1.1, col="blue")
```

```{r, fig.height=4, echo=T}
plot(AirQuality, col="blue")
abline(h=25)
```


* * * *
Visual Point & Click
========================================================

- R-Commander: looks like a 'normal' program  
  - Drop-down menus
  - Good for: Graphs, Regression, Correlation  
  - Judy Crane  
  <img src="http://socserv.mcmaster.ca/jfox/Misc/Rcmdr/Rcmdr-screenshot.jpg" height="200px" width="450px" alt="R commander screenshot"/>
   
- Downsides
   - Still need to process data
   - Graphics more limited
   - Miss out on R's super powers
- RStudio is a happy medium


* * * *                                                 
Intro Tutorials
========================================================
<img src="https://cloud.githubusercontent.com/assets/6283030/3576439/1be9db28-0b92-11e4-83e2-bb99a4826c10.JPG" height="200px" width="550px" alt="TryR screenshot"/>  

- Interactive Pirate Tutorial aRRRg! -> [TryR at CodeSchool](http://tryr.codeschool.com/levels/1/challenges/1)

- Follow Along Slide Shows by IDEM
 - [Basics: plot and load data](http://rpubs.com/NateByers/introRidem)
 - [Basics: summary statistics](http://rpubs.com/NateByers/introR2)
 - [Clean, Combine, Reshape and Filter data](http://rpubs.com/NateByers/manipRidem)
 - [Create own functions](http://rpubs.com/NateByers/introR3)
- [Data Camp](https://www.datacamp.com/courses)

                                                      
* * * *
The Next Step
========================================================

- R help, '''?median'''
  - `plot(` <push tab> 
- [Rseek.org](rseek.org)
- [StackOverflow](so.org)
- [R-bloggers](r-bloggers.org)
- [Quick-R](http://www.statmethods.net/)

- UCLA has a great <a href="http://www.ats.ucla.edu/stat/r/" target="_blank">website</a> for learning R and statistics
- There are many good books as well, such as
- <a href="http://www.amazon.com/Beginners-Guide-Use-Alain-Zuur/dp/0387938362/ref=sr_1_1?ie=UTF8&qid=1397750360&sr=8-1&keywords=beginner%27s+guide+to+R" target="_blank">Zuur et al.'s</a>
- <a href="http://www.amazon.com/Introductory-Statistics-R-Computing/dp/0387790535/ref=sr_1_1?ie=UTF8&qid=1397750420&sr=8-1&keywords=introductory+statistics+R" target="_blank">Dalgaard's</a>
- and <a href="http://www.amazon.com/Introductory-Beginners-Guide-Visualisation-Analysis-ebook/dp/B00BU34QTM/ref=sr_1_1?ie=UTF8&qid=1397750458&sr=8-1&keywords=introductory+R" target="_blank">Knell's</a>
- And remember, R can be freely <a href="http://www.r-project.org/" target="_blank">downloaded</a> and works on most operating systems

* * * *
Manuals
========================================================

Overview  
- [A Very Short Introduction to R pdf] (http://cran.r-project.org/doc/contrib/Torfs+Brauer-Short-R-Intro.pdf)  
- [R-intro pdf] (http://cran.r-project.org/doc/manuals/R-intro.pdf)  
- Reference Card of handy commands:  [R RefCard](https://github.com/jonasstein/R-Reference-Card/blob/master/R-refcard.pdf?raw=true)  

Special Topics  
 - Filter / Subset / Select Data     --> [Subsetting by Hadley Wickham](http://adv-r.had.co.nz/Subsetting.html)  
 - Time Series, Dates, and Air Data  --> [Open Air Project](http://www.openair-project.org/PDF/OpenAir_Manual.pdf)  
 - Spatial Data and Maps             --> [ggmaps by Wickham](http://journal.r-project.org/archive/2013-1/kahle-wickham.pdf)    
 - Cooperate, Document, and Share    --> [Don’t R Alone!](http://www.noamross.net/blog/2013/1/7/collaborating-with-r.html)   
 

Advanced
 - [Style Guide by Wickham](http://adv-r.had.co.nz/Style.html)
 - [Vocab List by Wickham](http://adv-r.had.co.nz/Vocabulary.html)
 - [Shiny Web Apps](http://shiny.rstudio.com/)

 
* * * *    
Videos and Courses
========================================================

- Two Minute Tutorials: [TwoTorials.com](twotorials.com)

Online Courses (Free)
 -  [Data Scientist’s Toolbox:]() This course gives an introduction to the main tools and ideas in
the data scientist's toolbox. The course gives an overview of the data,
questions, and tools that data analysts and data scientists work with.
There are two components to this course. The
 first is a conceptual introduction to the ideas behind turning data
into actionable knowledge. The second is a practical introduction to the
 tools that will be used in the program like version control, markdown,
git, GitHub, R, and RStudio.

- [Exploratory Data Analysis:]() This
 course covers the essential exploratory techniques for summarizing
data. These techniques are typically applied
 before formal modeling commences and can help inform the development of
 more complex statistical models. Exploratory techniques are also
important for eliminating or sharpening potential hypotheses about the
world that can be addressed by the data. We will
 cover in detail the plotting systems in R as well as some of the basic
principles of constructing data graphics. We will also cover some of the
 common multivariate statistical techniques used to visualize
high-dimensional data.

- [Reproducible Research:]()  After successfully completing this course you will be able to make visual representations of data using the base, lattice, and ggplot2 plotting systems in R, apply basic principles of data graphics to create rich analytic graphics from different types of datasets, construct exploratory summaries of data in support of a specific question, and create visualizations of multidimensional data using exploratory multivariate statistical techniques.

- [R programming:]() The course covers practical issues in statistical computing which includes programming in R, reading data into R, accessing R packages, writing R functions, debugging, profiling R code, and organizing and commenting R code. Topics in statistical data analysis will provide working examples.

- [Computing for Data Analysis:]() This course is about learning the fundamental computing skills necessary for effective data analysis. You will learn to program in R and to use R for reading data, writing functions, making informative graphs, and applying modern statistical methods.


* * * *     
Books
========================================================
Request to the Library 
```{r, eval=F} 
show(books)
```  

.....................Highlights......................... 


| Title | Author | Year |
|-------|--------|------| 
| The R Book | Michael Crawley | 2012 |
| [R Graphics Cookbook](http://www.amazon.com/R-Graphics-Cookbook-Winston-Chang/dp/1449316956) | Winston Chang | 2013 |
| Learning R  | Richard Cotton  | 2013 | 
| R Cookbook | Paul Teetor | 2011 |  
| R in a Nutshell| Joseph Adler | 2012 |  
| The Art of R Programming | Norman Matloff | 2011 | 
| Data Manipulation with R | Phil Spector | 2008 | 
| Ecological Models and Data in R *(Free)*  | Benjamin M. Bolker | 2008 |   
.................  .....................  
   
   
####[For more! Look **here** for an up-to-date Comprehensive list: http://www.r-project.org/doc/bib/R-books.html](http://www.r-project.org/doc/bib/R-books.html)

  
  
* * * *
MPCA Help
========================================================

- Stats Group Mentors
- Data Desk
- Live training in the works!

```{r, eval=F} 
ask_a_question(time = now!!, name = mr.Know.it.All, faster=better, help = "Yes, please")
```


  
* * * *  
Door Prize
=========================================================

```{r}

# Who's the lucky winner?
stats_Members <- c("Jim", "Kristie", "Jen")
sample(stats_Members, 1)

```

  
* * * *  
Credits
======================================================
- This document was created using RStudio's <a href="http://rmarkdown.rstudio.com/" target="_blank">"R Markdown"</a>
- RStudio can also be freely <a href="http://www.rstudio.com/" target="_blank">downloaded</a>
- The code for this presentation can be found here: <a href="https://github.com/mn-stats/Learning-R" target="_blank"> github.com/mn-stats/Learning-R/</a>
