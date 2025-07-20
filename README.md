# Central Limit Theorem Meets the Exam Room
author: Jędrzej Wydra

## Short summary:
Verified the Central Limit Theorem by simulating sample means from various distributions (uniform, t, chi-squared, Weibull, binomial, Poisson), showing convergence to normality as sample size increased.

## Technical summary:
Used NumPy, SciPy, and Matplotlib to generate synthetic samples, compute grouped sample means, and visualize their distributions. Verified asymptotic normality via simulation, highlighting reduced variance with larger sample sizes. No advanced metrics beyond visual convergence; focused on empirical illustration of CLT behavior.

## History
It started as a simple experiment to double-check whether the Central Limit Theorem really works. Spoiler: it does. I took samples from uniform, t, chi-squared, Weibull, binomial, and Poisson distributions, then created new samples from the means of increasingly larger groups. Sure enough, as sample sizes grew, those means started looking suspiciously normal.

But then I wondered — how does this play out in real life? Say, during exams. What if the number of questions on a test changes how much luck affects your grade? Turns out, it does. Thanks to the CLT, the more questions you get, the more your score reflects your actual knowledge, not just whether you guessed well (or got very unlucky). So if you're well-prepared, you should root for long exams. If you're not... maybe hope for just five questions and a miracle.

## Side Note
One thing that always makes me a little sad: how often the Central Limit Theorem gets misunderstood. No, it doesn’t magically turn your big sample into something normally distributed. What it does do is make the distribution of the *sample mean* approximately normal — big difference. Large samples just help you estimate the *true* distribution more precisely. So no, your messy, skewed data doesn’t suddenly become bell-shaped just because you collected more of it. Sorry!
