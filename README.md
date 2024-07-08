# Demonstration of the Central Limit Theorem

The Central Limit Theorem states that the distribution of the sample averages will approach a normal distribution as the sample size increases, regardless of the shape of the original distribution. The aim of [this](CLT_code.ipynb) notebook is to demonstrate this theory using the exponential distribution.
<br><br>
Let $X_{1}, X_{2}, ..., X_{n}$ be i.i.d. exponential random variables with parameter $\lambda$. If the CLT is indeed true, then we should get the following result for a sufficiently large $n$ :

$$
P\left(\bar{X}_n \geq \frac{1}{\lambda}\right) \approx P\left(\frac{1}{\lambda} \left(\frac{Z_n}{\sqrt{n}} + 1\right) \geq \frac{1}{\lambda}\right) = P\left(\frac{Z_n}{\sqrt{n}} + 1 \geq 1\right) = P\left(Z_n \geq 0\right)
$$

Where $Z_n \sim N(0,1)$, $\bar{X}_{n}$ is the sample average, and $\frac{1}{\lambda}$ is the true mean of the exponential distribution.

[histogram_of_sample_averages](histogram_of_sample_averages.png)

*Figure 1: Histogram of sample averages from the exponential distribution*
