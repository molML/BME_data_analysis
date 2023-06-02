---
layout: default
title: Introduction to data analysis
parent: Data analysis
nav_order: 1
---



# Navigation Structure
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---

## How to think about data


## Things to keep in mind


### Noise and error in biomedical data

Errors and noise are two common sources of variability that can impact the accuracy and reliability of biomedical data. 
Understanding the differences between these two types of variability is crucial for ensuring that research findings and 
clinical decisions are based on high-quality data.

*Error* refers to the difference between the true value or state of a measurement or observation and the recorded or 
measured value or state. These can arise from a variety of sources, including measurement error, sampling error, 
data entry error, and observer bias. Errors are typically systematic and non-random, and can be minimized through 
careful experimental design and data collection protocols.

<p align="center">
<img src="https://d20khd7ddkh5ls.cloudfront.net/types_of_error_flow_chart.jpeg" width=500>
</p>
<sup>Image credits [Caroline Monahan](https://www.expii.com/t/types-of-error-overview-comparison-8112) </sup>

*Noise*, on the other hand, refers to random or stochastic fluctuations in the data that are not related to the 
underlying biological signal or phenomenon of interest. This can arise from a variety of sources, 
including biological variability, measurement noise, and motion artifacts. 
Noise is typically random and non-systematic, and can be minimized through signal processing techniques such as 
filtering or averaging.

Both errors and noise can impact the validity and reliability of biomedical data, and it is important to carefully 
consider both sources of variability when analyzing and interpreting data. 
By understanding the differences between these two types of variability and implementing appropriate strategies for minimizing 
their effects, researchers and data analysis can ensure that their findings and decisions are based on data that are as high-quality, 
accurate, and reliable as possible.

### Simpson's paradox

Simpson's paradox is a statistical phenomenon that challenges our intuition and understanding of data analysis. It 
occurs when a trend or association observed within different subgroups of a dataset is reversed or even eliminated when 
the subgroups are combined. In other words, the relationship between two variables can appear to be one way when examined 
separately, but when the data is aggregated, the relationship flips or disappears entirely. Simpson's paradox highlights 
the importance of carefully considering the effects of confounding variables and the potential biases that can arise when interpreting data. It serves as a reminder that drawing conclusions based solely on aggregated data can lead to misleading or incorrect interpretations.


<p align="center">
<img src="https://miro.medium.com/v2/resize:fit:1100/format:webp/1*8tP_5zRKNAyVSeexu7RJZg.png" width=500>
</p>
<sup>Image credits: https://towardsdatascience.com/simpsons-paradox-and-interpreting-data-6a0443516765 </sup>

### Correlation vs causation
Correlation and causation are two distinct concepts in the realm of statistics and research. Correlation refers to a 
statistical relationship between two variables, indicating how they tend to vary together. It measures the strength and 
direction of the association between the variables, ranging from -1 (perfect negative correlation) to +1 (perfect positive
correlation), with 0 indicating no correlation. However, correlation alone does not imply causation. Causation, on the 
other hand, suggests that one variable directly influences or causes changes in another variable. It implies a 
cause-and-effect relationship, where a change in one variable leads to a predictable change in the other. Establishing 
causation requires more rigorous evidence, such as experimental design, controlling for confounding factors, and 
demonstrating temporal precedence. It is crucial to recognize that even though variables may be strongly correlated, 
there may be other factors at play that drive the relationship, making it a mere coincidence or a result of confounding 
variables. Therefore, caution must be exercised when inferring causation based solely on observed correlations.

<p align="center">
<img src="https://www.tylervigen.com/chart-pngs/2.png" width=500>
</p>
<sup>Image credits: https://www.tylervigen.com/spurious-correlations </sup>

## Multivariate data analysis



## Machine Learning




<sub>Copyright &copy; 2023 Francesca Grisoni. Distributed by an [MIT licence](LICENSE).</sub>

