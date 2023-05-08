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

#### Convex

* Let $X$ be a vector space. A subet $K$ of $X$ is ***convex*** if whenever $x,y\in K$ and $0\leq\lambda\leq 1$, we have $\lambda x+ (1-\lambda)y\in K$.

#### Minkowski's inequality in $\mathbb{R}^{n}$

* For all $1\leq p\leq\infty$, if $x,y\in\mathbb{R}^{n}$, then $$\left\|x+y\right\|_ {l^{p}}\leq\left\|x\right\|_ {l^{p}} + \left\|y\right\|_ {l^{p}}.$$

##### Equivalent norms

* Two norms $\left\|\cdot\right\|_ {1}$ and $\left\|\cdot\right\|_ {2}$ on $X$ are ***equivalent*** if there exists constants $0 \leq c_{1}\leq c_{2}$ such that $$c_{1} \left|x\right|_ {1}\leq\left|x\right|_ {2}\leq c_{2}\left|x\right|_ {1},$$ for every $x\in X$.

#### $l^{p}$ space

* The $l^{p}$ norm is given by $$\left\|x\right\|_ {l^{p}} = \left(\sum_{j=1}^{\infty}\left|x_{j}\right|^{p}\right)^{1/p}.$$

#### Minkowski's inequality in $l^{p}$

For all $1\leq p\leq\infty$, if $x,y\in l^{p}$ then $x+y\in l^{p}$ and $$\left\|x+y\right\|_ {l^{p}}\leq\left\|x\right\|_ {l^{p}} + \left\|y\right\|_ {l^{p}}.$$

#### $L^{p}$ space

* For $p\in [1,\infty)$, set $$\left\|f\right\|_ {L^{p}} = \left(\int_{a}^{b}\left|f(x)\right|^{p}\mathrm{d}x\right)^{1/p}.$$
