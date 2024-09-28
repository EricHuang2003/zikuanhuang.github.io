---
title: "Fiat-Shamir for Bounded-Depth Adversaries"
collection: publications
category: manuscripts
venue: 'Cryptology ePrint Archive'
coauthor: 'Liyan Chen, Yilei Chen, Nuozhou Sun, Tianqi Yang, Yiding Zhang'
paperurl: 'https://eprint.iacr.org/2024/256'
---

We study how to construct hash functions that can securely instantiate the Fiat-Shamir transformation against $\textbf{bounded-depth}$ adversaries. The motivation is twofold. First, given the recent fruitful line of research of constructing cryptographic primitives against bounded-depth adversaries under $\textbf{worst-case complexity assumptions}$, and the rich applications of Fiat-Shamir, instantiating Fiat-Shamir hash functions against bounded-depth adversaries under worst-case complexity assumptions might lead to further applications (such as SNARG for P, showing the cryptographic hardness of PPAD, etc.) against bounded-depth adversaries. 
Second, we wonder whether it is possible to overcome the impossibility results of constructing Fiat-Shamir for arguments  [Goldwasser, Kalai, FOCS '03] in the setting where the depth of the adversary is bounded, given that the known impossibility results (against p.p.t. adversaries) are contrived.

Our main results give new insights for Fiat-Shamir against bounded-depth adversaries in both the positive and negative directions.
On the positive side, for Fiat-Shamir for proofs with certain properties, we show that weak worst-case assumptions are enough for constructing explicit hash functions that give $\mathsf{AC}^0[2]$-soundness. In particular, we construct an $\mathsf{AC}^0[2]$-computable correlation-intractable hash family for constant-degree polynomials against $\mathsf{AC}^0[2]$ adversaries, assuming $\oplus\mathsf{L}/\mathsf{poly} \nsubseteq \widetilde{\mathsf{Sum}}_{n^{-c}} \circ \mathsf{AC}^0[2]$ for some $c > 0$. This is incomparable to all currently-known constructions, which are typically useful for larger classes and against stronger adversaries, but based on arguably stronger assumptions. Our construction is inspired by the Fiat-Shamir hash function by Peikert and Shiehian [CRYPTO '19] and the fully-homomorphic encryption scheme against bounded-depth adversaries by Wang and Pan [EUROCRYPT '22].

On the negative side, we show Fiat-Shamir for arguments is still impossible to achieve against bounded-depth adversaries. In particular,
\begin{itemize}
\item Assuming the existence of $\mathsf{AC}^0[2]$-computable CRHF against p.p.t. adversaries, for every poly-size hash function, there is a (p.p.t.-sound) interactive argument that is not $\mathsf{AC}^0[2]$-sound after applying Fiat-Shamir with this hash function.
\item Assuming the existence of $\mathsf{AC}^0[2]$-computable CRHF against $\mathsf{AC}^0[2]$ adversaries, there is an $\mathsf{AC}^0[2]$-sound interactive argument such that for every hash function computable by $\mathsf{AC}^0[2]$ circuits,
the argument does not preserve $\mathsf{AC}^0[2]$-soundness when applying Fiat-Shamir with this hash function. This is a low-depth variant of Goldwasser and Kalai.
\end{itemize}
