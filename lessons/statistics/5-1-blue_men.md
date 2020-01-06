[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```
# get the probabilities for men 5'10" and shorter and 6'1" and shorter
min_height = dist.cdf(177.8)
max_height = dist.cdf(185.4)
max_height - min_height
```
34% (0.3420946829459531)

First, I calculated the percentage of men with a height of 5'10" and shorter and 6'1" and shorter using the CDF. The difference between the two numbers results in the percentage of men in that height range.
