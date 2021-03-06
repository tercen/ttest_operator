# t-test operator

##### Description

The `ttest` operator performs a Student's t-test on the data.

##### Usage

Input projection|.
-----------|--------
`color`    | represents the groups to compare
`y-axis`   | measurement value
`labels`   | represents the pairing

Input parameters|.
---|---
`alternative`   | A character string specifying the alternative hypothesis, default is "two.sided"
`paired`        | logical, indicating whether to perform pairing, default FALSE
`mu`            | A number indicating the true value of the mean (or difference in means if you are performing a two sample test), default 0.0
`var.equal`     |logical, indicating whether to treat the two variances as being equal. If `TRUE` then the pooled variance is used to estimate the variance otherwise the Welch (or Satterthwaite) approximation to the degrees of freedom is used, default `FALSE`
`conf.level`    |numeric, confidence level of the interval, default 0.95

Output relations|.
---|---
`pv`| numeric, p-value calculated per cell

##### Details

The operator is the `t.test` function in base R.

##### References

see the `base::t.test` function of the R package for the documentation, 

##### See Also

[anova](https://github.com/tercen/anova_operator), [rfImp](https://github.com/tercen/rfImp_operator)

