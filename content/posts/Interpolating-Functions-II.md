---
title: "Interpolating Functions II"
---

In my previous post we discussed the Alexandrov-Hausdorff theorem, so we are now ready for Benyamini's beautiful paper ['Applications of the Universal Surjectivity of the Cantor Set'](https://www.jstor.org/stable/2589212?origin=JSTOR-pdf&seq=1). I first met this paper when it was referenced by Bayart and Quarta in a paper we will discuss later.

From here we will say a function $g:\mathbb{R} \rightarrow \R$ is $X$-universal (For $X \subseteq l^{\infty}$) if $\forall (x_n)_{n \in \N} \in X$ there is some $t \in \R$ such that $g(t+n) = x_n$ for all $n \in \N$.  

$$ \textbf{\textit{Theorem (Benyamini)}}$$ 
$$\textit{There exists a continuous l_{\infty}-universal function} g:\R \rightarrow \R$$
We will follow Benyamini's proof. Importantly, we will take $\mathfrak{C}$ as a subset of [0,$\frac{1}{2}$].

Define $K = \prod_{n \in \N}[-n,n]$. The space $K$ is a countable product of compact metric spaces, so is compact and metrizable. Now by the Alexandrov-Hausdorff Theorem (See my previous post) we get some continuous surjection $\phi: \mathfrak{C} \rightarrow K$. 
Now $\mathfrak{C}+n \cap \mathfrak{C}+m = \emptyset$ for $n,m \in \Z$ with $n \neq m$ (Recall how we defined $\mathfrac{C}$ above). Define $D = \bigsqcup_{n \in \N}\mathfrak{C}+n$. We first define $f: D \rightarrow \R$ by $$f(t+n) = \rho_n(\phi(t))$$ where $\rho_n$ denotes the projection from the $n$th coordinate onto $\R$. On the disjoint copies of $\mathfrak{C}$, we see $f$ is a composition of two continuous maps, so $f$ is continuous and well-defined. 

Now extend $f$ to a function $g:\R \rightarrow \R$, using the [Teitze Extension Theorem](https://en.wikipedia.org/wiki/Tietze_extension_theorem). We can now show that $g$ is $l_{\infty }-universal$. For any $(x_n)_{n \in \N} \in l_{\infty }$, as $\phi$ is surjective, that there exists some $t \in [0,\frac{1}{2}]$ such that $\phi(t) = $(x_n)_{n \in \N}$. By construction, we then have $g(t+n)= x_n$ for all $n \in \N$, as required. $\square$

Now the natural question is; how many of these functions are there? As we very rarely meet these functions in our day to day lives, one might think there are not very many at all! This intuition can be misleading, for example consider that the set of continuous nowhere differentiable functions on [0,1] (which we could perhaps call $ND[0,1]$) is dense in $C[0,1]$. One can also show $ND[0,1]$ is a very large subset of $C[0,1]$ in different measure-theoretic senses. 

This question will be answered in my next post in two different ways: In an algebraic way by Bayart and Quarta, and by Lars Olsen, Nathaniel Strout, and myself in a topological way. 
