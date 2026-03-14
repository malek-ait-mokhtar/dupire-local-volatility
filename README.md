# Dupire Local Volatility Model

Numerical study of the **Dupire local volatility model** for European option pricing.

This project investigates the mathematical framework and numerical resolution of the **Dupire partial differential equation**, which describes the evolution of option prices when volatility depends on strike and maturity.

---

## Model

In the local volatility framework, the underlying asset follows a diffusion of the form

\[
\frac{dS_t}{S_t} = (r_t - q_t)dt + \sigma_{loc}(S_t,t)dW_t
\]

The price of a European call \(C(K,T)\) then satisfies the **Dupire forward PDE**

\[
\partial_T C(K,T) =
\frac{1}{2}\sigma_{loc}^2(K,T)K^2 \partial_{KK}C(K,T)
\]

This formulation makes it possible to construct a diffusion process consistent with the full surface of market option prices.

---

## Repository

The repository contains two main components:

**Report**  
`dupire_modele_volatilite_locale_rapport.pdf` (Original report in French) 
Mathematical derivation of the Dupire equation, theoretical analysis and discussion of the numerical approach.

**Code**  
`méthodes_numériques_dupire.ipynb` (Original Notebook in Frenchs)
Python implementation of the numerical resolution of the Dupire PDE and generation of option price surfaces.

---

## Author

Malek Aït-Mokhtar  
PDE Project — 2026
