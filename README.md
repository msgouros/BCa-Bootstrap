# BCa-Bootstrap
__Statistic:__ Bootstrapping and bias-corrected accelerated bootstrap intervals 

__Data:__ Crime Files from University of Denver

__Background__: Bootstrapping is a statistical method that allows us to make inferences from a sample by resampling from the sample (with replacement).  When we do this many, many times (n=10,000), we are in a sense simluating what the underlying population would be by replicating from the sample.

Bootstrapping allows us to assign measures of accuracy (i.e., bias, variance, confidence intervals) to the sample estimates.  When it comes to coming up with confidence intervals on a bootstrap sample, there are different options; the percentile interval is a "first-order" interval that is formed from quantiles.  The percentile interval has two limitations: one, it is based on the bootstrap resamples (not the original data), and secondly, it does not take adjust for skew (if there is any in the bootstrapped resamples).

The BCa addresses both of these issues.  The code in this repository provides the analysis of a specific crime category at the University of Denver and illustrates the method of using bootstrapping.  It then shows how to use BCa to provide confidence intervals with a resampling population that has skew.  
