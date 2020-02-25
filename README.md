# Genes-Lefthandedness

This script explores the link between gene expression and left-handedness in a small dataset (n = 37) with correlational methods and
ordinal logistic regression.

The 'claridge' dataset was retrieved from: https://vincentarelbundock.github.io/Rdatasets/datasets.html
More info: https://vincentarelbundock.github.io/Rdatasets/doc/boot/claridge.html

The dataset contains two variables: 'genetic expression' (generally but not specifically defined) which is hypothetically linked to lefthandedness, and self-report rating of participant for their left-handedness from 1 (not left-handed) to 8 (very left-handed).

Histogram of both genetic expression and left-handedness was conducted to examine the distribution. For the histogram of left-handedness ratings, the distribution was very skewed to the left (positive skew); this is not incredibly surprising as most of the population is right-handed, not left-handed. 

Due the small sample size and this positive skew, I selected spearman's method of correlation to reduce to the effect of outliers and better fit ordinal vs continuous data. A correlation test was computed to calculate the p-value for the spearman correlation.

I attempted another method of using ordinal logistic regression using the 1-8 lefthanded scale as ordered factors, and then subsequently computed the p-values. However, this method may have been problematic because of the lack of any data points for '7' rating of left-handedness. 

