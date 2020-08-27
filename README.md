# Machine_Learning_tutorial_2
The tutorial will help budding data scientists get familiar with machine learning concepts

Anomaly Detection

we will implement an anomaly detection algorithm using the Gaussian model to detect anomalous behavior in a 2D dataset first and then a high-dimensional dataset.

we are going to use Gaussian distributions to model the data. To accomplish this, we are going to introduce scipy, a package which contains a wide variety of tools for working with scientific data in Python. Its stats package allows us to easily model various statistical distributions, and get information about them.

Scipy's Gaussian distribution class is called norm. It takes two parameters - loc, which corresponds to the mean of your distribution, and scale, which corresponds to the standard deviation.

Also,
we will use the following formula to calculate the probability of each point, and set it to `p`:

p(x)=1−(∏i=1k1−p(x∈k))

This formula returns the probability that the datapoint was produced at random by _any_ of the Gaussians we fit. Hence, we want to filter out anything without a very high probability of this.
