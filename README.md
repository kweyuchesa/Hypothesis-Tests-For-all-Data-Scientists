## Hypothesis-Tests-For-all-Data-Scientists

  Hypothesis testing is one of the most fundamental elements of inferential statistics. In modern languages like Python and R, these tests are easy to conduct — often with a single line of code. But it never fails to puzzle me how few people use them or understand how they work. In this repository I would like to use an example to show three common hypothesis tests and how they work under the hood, as well as showing how to run them in R and Python and to understand the results.

## The general principles and process of hypothesis testing
  Hypothesis testing exists because it is almost never the case that we can observe an entire population when trying to make a conclusion or inference about it. Almost always, we are trying to make that inference on the basis of a sample of data from that population.

  Given that we only ever have a sample, we can never be 100% certain about the inference we want to make. We can be 90%, 95%, 99%, 99.999% certain, but never 100%.

Hypothesis testing is essentially about calculating how certain we can be about an inference based on our sample. The most common process for calculating this has several steps:

  1. Assume the inference is not true on the population — this is called the null hypothesis
  2. Calculate the statistic of the inference on the sample
  3. Understand the expected distribution of the sampling error around that statistic
  4. Use that distribution to understand the maximum likelihood of your sample statistic being consistent with the null hypothesis
  5. Use a chosen ‘likelihood cutoff’ — known as alpha — to make a binary decision on whether to accept the null hypothesis or reject it. The most commonly used value of alpha is 0.05. That is, we usually reject a null hypothesis if it renders the maximum likelihood of our sample statistic to be less than 1 in 20.

We are going to use ~salespeople dataset to illustrate this important statistical concept. 
