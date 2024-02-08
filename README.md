# Computational Intensive Stats: Project 01

__Course Code: STA 6106__
__Period: Spring 2024__ \
__Instructor: Dr. Ping Sa__ \
__Textbook: Simulation, 6th Ed. by Sheldon M. Ross__


The Course description and other information can be found among the following links: 
* Degree Requirements: https://www.unf.edu/catalog/programs/gr/coas/COAS-MSAMATMAT1.html 
* Course Catalogue: https://www.unf.edu/catalog/courses/?level=gr#
* Textbook: https://shop.elsevier.com/books/simulation/ross/978-0-323-85738-3

# Assignment Statement

One simple test to determine whether a random number generator is giving random values from a distribution with distribution function $F(x)$ is that of Kolmogorov and Smirnov. 

Using the random number generator, obtain a sample of size $n$. 

Order the sample with $x_r$ being the $r^{\text{th}}$ smallest observation. 

Define the sample distribution function $S_n$ to be 

$$
S_n(x) =  
\begin{cases} 
  0 \text{ for } x < x_{(1)} \\ 
  \frac{r}{n} \text{ for } x_{(r)} \leq x < x_{(r+1)} \\
  1 \text{ for } x_{(n)} \leq x 
\end{cases}
$$

Then, for $n$ larger than $80$, it can be shown that if the $x$'s are truly coming from $F$, then, with probability $0.99$, 

$$\text{sup}_x \vert S_n(x) - F(x) \vert < \dfrac{1.6276}{\sqrt{n}}.$$

## Minimal Requirement (80%):

Use the random number generator, $X_{n+1} = 7^5 X_n \text{mod}(2^{31} -1)$, to generate a sample of size $1,000$ from the uniform distribution on the unit interval.

Does your sample pass the Kolmogorov-Smirnov test?

## Additional Requirements (10%):

The above is the minimal requirement, but please extend your study to truly answer the question: Does the random number generator generate uniform distribution on the unit interval?

## Completeness Requirements (10%):

The written report should include a complete description of the problem, a description of the Monte Carlo teqchniques used, the results of the Monte Carlo simulations, and your conclusions.

A program listing and output should be included as an appendix.

Neatness, organization, and clarity will count 10% of the project grade.
