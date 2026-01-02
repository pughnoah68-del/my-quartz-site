---
title: "Hello World"
---

My first series of posts will build to a result Nathaniel Strout, Lars Olsen and I proved about a set of very interesting functions, which will be introduced along the way.


The story begins with the Alexandrov-Hausdorff theorem. I had never heard of Alexandrov before coming across this theorem, and [his MacTutor article](https://mathshistory.st-andrews.ac.uk/Biographies/Aleksandrov/) makes for an interesting read. Setting off alarm bells, there is a quote about his swimming habits: 'Every day Aleksandrov and Urysohn swam across the Rhine - a feat that was far from being safe and provoked Hausdorff's displeasure'. Wikipedia claims they were swimming together in Batz-sur-Mer when Urysohn drowned!

$$ \textbf{\textit{Theorem (Alexandrov, Hausdorff)}}$$ 
$$\textit{Every compact metrizable space is the continuous image of the Cantor set } \mathfrak{C}.$$

Kechris’s Descriptive Set Theory gives a very neat proof, but makes use of some helpful preliminaries:

Let $X$ our compact metrizable space be given. We may assume $X$ has some metric $d$ with image contained in $[0,1]$. From a standard fact of topology, every compact metric space is separable, so we may find some countable dense set $ (x_n)_{n \in \mathbb{N}}$.

We now need to define some important maps. First define $ f:X \rightarrow [0,1]^{\mathbb{N}}$ where $f(x) = (d(x,x_n))_{n \in \mathbb{N} } $. This map is continuous and injective, so $ X \cong im(f):= F$.
Then there is the surjective map $ g': \mathfrak{C} \rightarrow [0,1]$ where $ g'(a)= \sum_{n \in \mathbb{N}} 2^{-n-1}a_n$ where $ a=0.a_{1}a_{2}...$ in base 3. The function$ g'$ can be viewed as taking an element’s base 3 representation and pretending that it was a base 2 representation. Now $ g'$ can be extended to a surjective map $ g: \mathfrak(C)^{\mathbb{N}} \rightarrow [0,1]^{\mathbb{N}}$, and we can note $\mathfrak(C)^{ \mathbb{N} } \cong \mathfrak(C)$.
So bringing these together we have a continuous surjection from $ g^{-1}(F)$ onto $X$. Thus, we will be done if we can show $ g^{-1}(F) \subseteq \mathfrak{C}$ admits a retraction. Kechris gives a more general version of this result using trees, but there is a nice idea for this closed subspaces of $\mathfrak{C}$: For each $ x \in \mathfrak{C}$ there is some unique $k_x \in K$ such that $ d(x,k_x) = d(x,K)$. The map $x \mapsto k_x$ is then our desired retraction. $\square$


In my next post, I will discuss how Benyamini goes on to explore some interesting and counter-intuitive consequences of this theorem, which will hopefully shock the reader as much as it did Nathaniel, Lars and I.


In a fun related note, Dreher and Samuel in [arXiv:1303.3810v2](https://arxiv.org/pdf/1303.3810) give a countable compact space which is not a continuous image of $ \mathfrak{C}$. I think before having a look, one should dust off Counterexamples in Topology and play around for a while.