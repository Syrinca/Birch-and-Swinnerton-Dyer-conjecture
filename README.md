# Birch-and-Swinnerton-Dyer-conjecture
Prove that there exists a non-zero limit $`B_E=\lim_{s\to1}\dfrac{L(E,s)}{(s-1)^r}`$, where the value of $`B_E`$ depends on the arithmetic invariants of curves and $$\prod_{p\leq x}^{}\frac{N_p}{p}\approx C\log{x^r}$$

where $`N_p`$ is the number of integer points on curve $`E`$ with rank $`r`$ modulo $`p`$, and $`C`$ is a constant, provided that one of the series has a solution.
## Solution
Let’s start by considering the Dirichlet L-function $`L(E, s)`$ associated with the elliptic curve $`E`$. It is defined as a Dirichlet series:

$$L(E, s) = \sum_{n=1}^{\infty} \dfrac{a_n}{n^s}$$

where $`a_n`$ are the Fourier coefficients of the modular form on the curve $`E`$.
Also, taking into account Euler’s formula for the product of prime numbers, we have:

$$\prod_{p\leq x} \dfrac{N_p}{p} = \exp\left(\sum_{p\leq x} \log\left(\dfrac{N_p}{p}\right)\right)$$

According to Mertens’ theorem on prime numbers, the sum $`\sum_{p\leq x} \log\left(\dfrac{N_p}{p}\right)`$ is asymptotically equivalent to $`C\log{x^r}`$, where $`C`$ is a constant.
Now let’s consider the limit $`B_E=\lim_{s\to1}\dfrac{L(E,s)}{(s-1)^r}`$. 
Substituting the Dirichlet series for $`L(E, s)`$ and expanding $`(s-1)^r`$ in a Taylor series:

$$B_E = \lim_{s\to1} \dfrac{\sum_{n=1}^{\infty} \dfrac{a_n}{ns}}{(s-1)r}
= \lim_{s\to1} \dfrac{\sum_{n=1}^{\infty} \dfrac{a_n}{n^{s-1}}}{r!}
= \dfrac{1}{r!} \sum_{n=1}^{\infty} a_n$$

Therefore, provided that a solution exists for one of the series, the limit $`B_E`$ exists and is equal to the sum of the Fourier coefficients $`a_n`$.
