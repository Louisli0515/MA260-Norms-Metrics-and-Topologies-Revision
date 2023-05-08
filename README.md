# MA260-Norms-Metrics-and-Topologies-Revision
My own notes about the MA260 revision, mainly from the notes and example sheets

## Lecture notes

[260_notes_2022-23.pdf](https://github.com/Louisli0515/MA260-Norms-Metrics-and-Topologies-Revision/files/11422967/260_notes_2022-23.pdf)

First of all, feel free to download 2022-2023 lecture notes for MA260.

## Example sheets

For the second term revision, I will combine all the examples into one pdf, and therefore we will not use sub-headings for each week but instead just topics.

### Countable

* A set $A$ is countable if it is in bijection with a subset of $\mathbb{N}$ or, equivalently, if there is an injection from $A$ to $\mathbb{N}$. A countable set may be finite or infinite, in which case we call it countably infinite. 
* The empty set is countable.

### Norms

A norm on a vector space $X$ is a map $\left|\cdot\right|:X\to\mathbb{R}^{+}$ such that 

* $\left\|x\right\| = 0$ if and only if $x = 0$.
* $\left\|\lambda x\right\| = \left|\lambda\right|\left\|x\right\|$ for every $\lambda\in\mathbb{R}$ or $\mathbb{C}$, $x\in X$ ('homogeneity') and 
* $\left\|x+y\right\|\leq\left\|x\right\|+\left\|y\right\|$ for every $x,y\in X$ (the triangle inequality).

#### Standard norm/Euclidean norm

* In the vector space $\mathbb{R}^{n}$, for $x = (x_{1},x_{2},...,x_{n})$ define $$\left\|x\right\| = \left(\sum_{j=1}^{n}\left|x_{j}\right|^{2}\right)^{1/2},$$ the standard norm or Euclidean norm.
* There are other norms on $\mathbb{R}$. For example, $$\left\|x\right\|_ {l^{1}} = \sum_{j=1}^{n}\left|x_{j}\right|$$ and $$\left\|x\right\|_ {l^{\infty}} = \max_{j=1,...,n}\left|x_{j}\right|.$$

#### Normed space

* If $X$ is a vector space and $\left\|\cdot\right\|$ is a norm on $X$, the pair $(X,\left\|\cdot\right\|)$ is a normed space.

#### Closed unit ball

* The closed unit ball in $(X,\left\|\cdot\right\|)$ is the set $$\mathcal{B}_{X} = \set{x\in X: \left\|x\right\|\leq 1}.$$
