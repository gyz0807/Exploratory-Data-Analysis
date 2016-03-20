Quiz 2
======

Question 2
----------

What is produced by the following code?

``` r
library(nlme)
library(lattice)
xyplot(weight ~ Time | Diet, BodyWeight)
```

![](Quiz_2_files/figure-markdown_github/Q2-1.png)<!-- -->

Question 7
----------

Load the \`airquality' dataset form the datasets package in R

library(datasets)
data(airquality)

I am interested in examining how the relationship between ozone and wind speed varies across each month. What would be the appropriate code to visualize that using ggplot2?

``` r
library(datasets); data(airquality); library(ggplot2)
airquality <- transform(airquality, Month = factor(Month))
qplot(Wind, Ozone, data = airquality, facets = . ~ Month)
```

![](Quiz_2_files/figure-markdown_github/Q7-1.png)<!-- -->

Question 10
-----------

The following code creates a scatterplot of 'votes' and 'rating' from the movies dataset in the ggplot2 package. After loading the ggplot2 package with the library() function, I can run

qplot(votes, rating, data = movies)

How can I modify the the code above to add a smoother to the scatterplot?

``` r
qplot(votes, rating, data = movies) + geom_smooth()
```

![](Quiz_2_files/figure-markdown_github/Q10-1.png)<!-- -->
