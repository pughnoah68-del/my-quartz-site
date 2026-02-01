---
draft: true
---

---
title: "Interpolating Functions II"
---

In my previous post we discussed the Alexandrov-Hausdorff theorem. We are now ready to discuss Benyamini's beautiful paper ['Applications of the Universal Surjectivity of the Cantor Set'](https://www.jstor.org/stable/2589212?origin=JSTOR-pdf&seq=1). I first met this paper when it was referenced by Bayart and Quarta in a paper we will discuss later.

We are interested in interpolating functions, but we should not skip past the following result, which will hopefully please all of my fellow St Andrews students who recently finished our discrete geometry course: 

$$ \textbf{\textit{Theorem (Grz\k{a}\'slewicz)}}$$ 
$$\textit{For all} d \geq 1 \textit{, there exists some compact convex set} B \subseteq \mathbb{R}^{d+2} \textit{such that every compact convex subset of the } d-\textit{cube is congruent to a face of B}.$$

We could call such a $B$ a universal compact convex subset. It is interesting to see why such a universal compact convex subset cannot lie in $\mathbb{R}^{d+1}$. 
From here we will say a function $f:\mathbb{R} \rightarrow \R$ is $X$-interpolating (For $X \subseteq l^{\infty}$) if $\forall (x_n)_{n \in \N} \in X$ there is some $t \in \R$ such that $f(t+n) = x_n$ for all $n \in \N$.  

$$ \textbf{\textit{Theorem (Benyamini)}}$$ 
$$\textit{There exists a universally interpolating function}$$

$$
