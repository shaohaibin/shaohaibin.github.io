---
layout: default
---


<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/3.4.12/d3.js"></script>
<!-- <script src="{{site.baseurl}}/js/embed-d3.js"></script> -->


### Topics ###

## Neighbor selection: less connected, better convergence.

<img src="../../../images/NS.png" width="400"  />

In this thread of works, we ask:

***How the convergence rate of a diffusively coupled multi-agent network can be drammatically enhanced with less communication links?***

We have established the following results:

1. ***Global network connectivity guarantee via distributed neighbor selection.***
2. ***Convergence rate of the on the multi-agent system on the simplified network can be drammatically enhanced.*** 


#### Magic Eigenvector

<span style="color:red;"> Relative Tempo Theorem </span> (Bridging the Local Relative State and Network Eigenvectors, e.g., Fiedler Vector)

Consider the following ordinary differential equations on a simple graph $$\mathcal{G} = (\mathcal{V},\mathcal{E},A)$$, 

$$ \dot{\boldsymbol{x}}_{i}(t)=-\sum_{j=1}^{|\mathcal{V}|}a_{ij}\left(\boldsymbol{x}_{i}(t)-\boldsymbol{x}_{j}(t)\right), i\in\mathcal{V},$$

where $$\mathcal{V}=\{1,2,\cdots,n\}$$, $$A=[a_{ij}] \in \mathbb{R}^{n \times n}$$ is the [adjacency matrix](https://en.wikipedia.org/wiki/Adjacency_matrix) of $$\mathcal{G}$$.

Then

$$\lim_{t \rightarrow \infty} \frac{\|\dot{\boldsymbol{x}}_{i}(t)\|}{\|\dot{\boldsymbol{x}}_{j}(t)\|} = \frac{\| [\boldsymbol{v}_{2}(L)]_i\|}{\| [\boldsymbol{v}_{2}(L)]_j\|},$$

where $$L$$ and $$\boldsymbol{v}_{2}(L)$$ are the [Laplacian](https://en.wikipedia.org/wiki/Laplacian_matrix) and the [Fiedler vector](https://en.wikipedia.org/wiki/Algebraic_connectivity) of $$\mathcal{G}$$, respectively.

#### Related Papers


1. **Haibin Shao**, Lulu Pan, Mehran Mesbahi, Yugeng Xi and Dewei Li.    
   [*Relative tempo of distributed averaging on networks*.](https://doi.org/10.1016/j.automatica.2019.03.004)     
    **Automatica**, 105:159-166, 2019. [PDF](https://doi.org/10.1016/j.automatica.2019.03.004)

2. **Haibin Shao**, Lulu Pan, Mehran Mesbahi, Yugeng Xi, Dewei Li.    
   [*Distributed Neighbor Selection in Multi-agent Networks*.](https://doi.org/10.1109/TAC.2023.3246425)    
   **IEEE Transactions on Automatic Control**, 68(11):6711-6726, 2023. [PDF](https://doi.org/10.1109/TAC.2023.3246425)

3. Lulu Pan, **Haibin Shao**, Mehran Mesbahi, Dewei Li, Yugeng Xi.    
   [*Structural Adaptivity of Directed Networks*.](https://arxiv.org/pdf/2208.13223)  
   arXiv preprint arXiv:2208.13223. [PDF](https://arxiv.org/pdf/2208.13223)
   
4. Haibin Shao, Merhan Mesbahi, Dewei Li, and Yugeng Xi. *[Inferring centrality from network snapshots](https://www.nature.com/articles/srep40642)*. **Scientific Reports**, 2017, 7(1):1-13.
