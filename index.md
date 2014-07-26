---
title       : Iris dataset data analysis
subtitle    : Analyzing linear correlations of the iris dataset
author      : Francisco Sokol
job         : Software Developer - Caelum - Brazil, Sao Paulo
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

--- .class #id 

## The iris dataset

The iris dataset is a collection of measurements collected from 
50 flowers of 3 different species.

This dataset is bundled with R, and can be examined with the `iris` variable.

The following variables are available in the dataframe:


```r
names(iris)
```

```
## [1] "Sepal.Length" "Sepal.Width"  "Petal.Length" "Petal.Width" 
## [5] "Species"
```

---
## The iris dataset

Here is a summary of the dataframe:


```r
summary(iris)
```

```
##   Sepal.Length   Sepal.Width    Petal.Length   Petal.Width 
##  Min.   :4.30   Min.   :2.00   Min.   :1.00   Min.   :0.1  
##  1st Qu.:5.10   1st Qu.:2.80   1st Qu.:1.60   1st Qu.:0.3  
##  Median :5.80   Median :3.00   Median :4.35   Median :1.3  
##  Mean   :5.84   Mean   :3.06   Mean   :3.76   Mean   :1.2  
##  3rd Qu.:6.40   3rd Qu.:3.30   3rd Qu.:5.10   3rd Qu.:1.8  
##  Max.   :7.90   Max.   :4.40   Max.   :6.90   Max.   :2.5  
##        Species  
##  setosa    :50  
##  versicolor:50  
##  virginica :50  
##                 
##                 
## 
```

---

## Linear correlations

When anlysing the whole dataset, there seems to be a some positive linear correlation
between Sepal and Petal Length:

![plot of chunk unnamed-chunk-3](assets/fig/unnamed-chunk-3.png) 

---

## Linear correlations

But when we partition the data between the three different species, we can see that
this correlantion is higher:

![plot of chunk unnamed-chunk-4](assets/fig/unnamed-chunk-4.png) 

