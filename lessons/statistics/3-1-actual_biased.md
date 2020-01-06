[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

**Code:**
```
resp = nsfg.ReadFemResp()

pmf = thinkstats2.Pmf(resp.numkdhh, label = 'actual')

thinkplot.Pmf(pmf)
thinkplot.Config(xlabel='# of Kids in HH', ylabel='PMF')
```
![Image of actual pmf]
(https://github.com/chrisjchung/dsp/blob/master/lessons/statistics/3-1_actual.png)

```
biased = BiasPmf(pmf, label = 'biased')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased])
thinkplot.Config(xlabel='# of Kids in HH', ylabel='PMF')
```
![Image of actualbiased pmf]
(https://github.com/chrisjchung/dsp/blob/master/lessons/statistics/3-1_actualbiased.png)

```
print('Actual', pmf.Mean())
print('Biased', pmf.Mean())
```
Actual 1.024205155043831

Biased 1.024205155043831


Similar to the example with the class size, the charts above show that the actual data differs from the observed set. In the actual data, a significant portion of the respondents don't have any kids in the househould, but since the observed data can only come from HHs with kids, there's a 0% probability in the observed.
