[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```
t = np.random.random(1000)

pmf = thinkstats2.Pmf(t)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Config(xlabel='Random number', ylabel='PMF')
```
![pmf_random](https://github.com/chrisjchung/ThinkStats2/blob/master/code/4-2_pmf_random.png)
```
cdf = thinkstats2.Cdf(t)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random number', ylabel='CDF')
```
![cdf_random](https://github.com/chrisjchung/ThinkStats2/blob/master/code/4-2_cdf_random.png)

Based on the distributions, there are so many values it becomes hard to distinguish when looking at the PMF, but the CDF makes it easier to see that there is relatively flat increase in the line, which indicates the distribution is, in fact, uniform.
