<!-- TITLE: Kernel Density Estimation -->
<!-- SUBTITLE: My understanding of Kernel Density Estimation -->

# What is Kernel?
The **Probability Density Function** is a function that used to specify the possibility of a continous random variable falling within a particular range of values (as apposed to taking on any value). This probability is given by the area under the density function but above the horizontal axis and between the lowest and greatest values of the range. An example probability density function is as below:

![Visualisation Mode Median Mean Svg](/uploads/machine-learning/visualisation-mode-median-mean-svg.png "Visualisation Mode Median Mean Svg"){.align-center}

And the Probability Density Function has the following properties: 
* non-negative everywhere 
* integral over the entire space is equal to 1 
* real-valued (continuous)

A **kernel** is a special type of Probability Density Function with the added property that it must be even. Some of the commonly used kernels are shown in the diagram below:
