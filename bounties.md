---
layout: home
---

# Legendre PRF bounties

## The Legendre PRF

The Legendre pseudo-random function is a one-bit PRF $$\mathbb{F}_p \rightarrow \{0,1\}$$ defined using the Legendre symbol:

$$ \displaystyle L_{p, K}(x) = \left\lceil\frac{1}{2}\left( \left(\frac{K + x}{p}\right) + 1\right)\right\rceil $$

## Bounties

### $ 10,000

&nbsp;&nbsp;For either

* a sub-exponential, i.e. $$2^{(\log p)^{o(1)}}$$, classical key recovery algorithm that extracts the key $$K$$ using inputs chosen by the attacker[^1]
* a security proof showing the non-existence of such an algorithm by reducing it to a well-established computational hardness assumption (see below)

### $ 3,000 

&nbsp;&nbsp;For a classical key recovery algorithm improving on the Russel-Shparlinski ($$O(p \log^2 p)$$ deterministic or $$O(p \log p)$$ probabilistic) algorithm, using a sub-exponential, i.e. $$2^{(\log p)^{o(1)}}$$ number of queries.[^1] [^2]

### $ 1,000

&nbsp;&nbsp;For the most interesting paper on the Legendre PRF in the next year (ends 31 August 2020)[^3]

[^1]: In all cases, probabilistic algorithms are also considered if they improve on the probabilistic versions of the known algorithms. Only classical (non-quantum) algorithms are permitted for the algorithm bounties.

[^2]: For this bounty, we also consider any algorithm that can distinguish a $$2^{(\log p)^{o(1)}}$$ bit length output of the Legendre PRF from a random bit string with advantage $$>0.1$$}

[^3]: A cryptographer will be appointed by the Ethereum Foundatoin to judge this (TBD)

Fhe first bounties are for the first entry that beats the given bounds. Please send submissions to Dankrad Feist dankrad .at. ethereum .dot. org.

## Computational hardness assumptions

For the reduction to a well-established computational hardness assumption, we consider the assumptions below which are taken from the [Wikipedia page](https://en.wikipedia.org/wiki/Computational_hardness_assumption)

* Integer factorization problem
* RSA problem
* Quadratic residuosity, higher residuosity and decisional composite residuosity problem
* Phi-hiding assumption
* Discrete logarithm, Diffie-Hellman and Decisional Diffie-Hellman in $$\mathbb{F}_p^{\times}$$
* Lattice problems: Shortest vector and learning with errors

## Concrete instances

TBA: Some bounties for key recovery in concrete instances will be announced soon, stay tuned.

### Research papers

* [Damgård, Ivan Bjerre: On The Randomness of Legendre and Jacobi Sequences (1988)](https://link.springer.com/content/pdf/10.1007%2F0-387-34799-2_13.pdf)
* [Lorenzo Grassi, Christian Rechberger, Dragos Rotaru, Peter Scholl, Nigel P. Smart: MPC-Friendly Symmetric Key Primitives (2016)](https://eprint.iacr.org/2016/542.pdf)
* [Alexander Russell, Igor Shparlinski: Classical and Quantum Polynomial Reconstruction via Legendre Symbol Evaluation (2002)](https://arxiv.org/pdf/quant-ph/0212016.pdf)
* [Dmitry Khovratovich: Key recovery attacks on the Legendre PRFs within the birthday bound](https://eprint.iacr.org/2019/862.pdf)

