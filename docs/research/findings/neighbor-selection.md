---
layout: default
---



<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/3.4.12/d3.js"></script>
<!-- <script src="{{site.baseurl}}/js/embed-d3.js"></script> -->


### Findings ###

# Less connected, but more functional

In this thread of works, we ask:

***how the performance of a cooperative multi-agent network can be drammatically enhanced with relatively less communications, which can be very expensive (e.g., underwater communication)?***

We have established the following results:

1. ***Global network connectivity via local neighbor selection.***
2. ***Convergence rate of reduced network can be drammatically enhanced.*** 


#### Magic Mathematics

<span style="color:red;"> Relative Tempo Theorem (Linking Local Relative State and Fiedler Vector, Ref.2)</span>

Consider the following ordinary differential equations on a simple graph $$\mathcal{G} = (\mathcal{V},\mathcal{E},A)$$, 

$$ \dot{\boldsymbol{x}}_{i}(t)=-\sum_{i=1}^{|\mathcal{V}|}a_{ij}\left(\boldsymbol{x}_{i}(t)-\boldsymbol{x}_{j}(t)\right), i\in\mathcal{V},$$

where $$\mathcal{V}=\{1,2,\cdots,n\}$$, $$A=[a_{ij}] \in \mathbb{R}^{n \times n}$$ is the [adjacency matrix](https://en.wikipedia.org/wiki/Adjacency_matrix) of $$\mathcal{G}$$.

Then

$$\lim_{t \rightarrow \infty} \frac{\|\dot{\boldsymbol{x}}_{i}(t)\|}{\|\dot{\boldsymbol{x}}_{j}(t)\|} = \frac{\| [\boldsymbol{v}_{2}(L)]_i\|}{\| [\boldsymbol{v}_{2}(L)]_j\|},$$

where $$L$$ and $$\boldsymbol{v}_{2}(L)$$ are the [Laplacian](https://en.wikipedia.org/wiki/Laplacian_matrix) and the [Fiedler vector](https://en.wikipedia.org/wiki/Algebraic_connectivity) of $$\mathcal{G}$$, respectively.

#### Related Papers

1. Haibin Shao, Lulu Pan, Mehran Mesbahi, Yugeng Xi and Dewei Li. **[Relative tempo of distributed averaging on networks](https://www.sciencedirect.com/science/article/abs/pii/S0005109819301256?via%3Dihub)**. **Automatica**, 2019, 105:159-166.
2. Haibin Shao, Lulu Pan, Mehran Mesbahi, Yugeng Xi, Dewei Li. **[Distributed Neighbor Selection in Multi-agent Networks](https://arxiv.org/abs/2107.12022)**. arXiv preprint arXiv:2107.12022.
3. Haibin Shao, Merhan Mesbahi, Dewei Li, and Yugeng Xi. **[Inferring centrality from network snapshots](https://www.nature.com/articles/srep40642)**. **Scientific Reports**, 2017, 7(1):1-13.
4. Lulu Pan, **Haibin Shao**, Dewei Li. **[Peer Selection in Opinion Dynamics on Signed Social Networks with Stubborn Individuals]((https://doi.org/10.1016/j.neucom.2021.12.105))**. **Neurocomputing**, 477:104-113, 2022.
