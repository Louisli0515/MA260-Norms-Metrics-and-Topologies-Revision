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

### Metric space

A metric $d$ on a set $X$ is a map $d:X\times X\to\mathbb{R}^{+}$ such that 

* $d(x,y) = 0$ if and only if $x = y$.
* $d(x,y) = d(y,x)$ for every $x,y\in X$ and 
* $d(x,z)\leq d(x,y)+d(y,z)$ for every $x,y,z\in X$ (triangle inequality).

#### Standard metric/Euclidean metric

* The standard metric or Euclidean metric on $\mathbb{R}^{n}$ is given by $$d_{2}(x,y) = \left\|x-y\right\|_ {l^{2}} = \left(\sum_{j=1}^{n}\left|x_{j}-y_{j}\right|^{2}\right)^{1/2}.$$

#### Discrete metric 

* The ***Discrete metric*** on any non-empty set $X$ is defined by setting $d(x,x) = 0$ and $d(x,y) = 1$ if $x\ne y$. (Useful in counterexamples)

#### Sunflower metric 

* The ***Sunflower metric*** on $\mathbb{R}^{2}$ is given by $d(x,y) = \left\|x-y\right\|$ if $x$ and $y$ lie on same line through the origin, and $\left\|x\right\|+\left\|y\right\|$ otherwise.

#### Jungle river metric

* The ***Jungle river metric*** on $\mathbb{R}^{2}$ is given by $d((x_{1},y_{1}),(x_{2},y_{2})) = \left|y_{1}-y_{2}\right|$ if $x_{1}= x_{2}$ and $d((x_{1},y_{1}),(x_{2},y_{2})) = \left|y_{1}\right|+\left|x_{1}-x_{2}\right|+\left\|y_{2}\right\|$ otherwise.

### Open and closed sets

* The ***Open ball*** centred at $a\in X$ of radius $r$ is the set $$\mathbb{B}(a,r) = \set{x\in X: d(x,a) < r}.$$
* The ***Closed ball*** centred at $a\in X$ of radius $r$ is the set $$\overline{\mathbb{B}}(a,r) = \set{x\in X: d(x,a)\leq r}.$$

#### Bounded subsets

* A subset $S$ of $(X,d)$ is ***bounded*** if there exists $a\in X$ and $r > 0$ such that $S\subset\mathbb{B}(a,r)$.

#### Open and closed subsets

* A subset $U$ of $(X,d)$ is ***open*** in $X$ if for every $x\in U$, there exists $\varepsilon > 0$ such that $\mathbb{B}(x,\varepsilon)\subset U$.
* A subset $F$ of $(X,d)$ is ***closed*** in $X$ if $X\setminus F$ is open.
* Open balls are open.
* If $U_{1},...,U_{n}$ are open in $(X,d)$, then $\displaystyle\bigcap_{i=1}^{n} U_{i}$ is open in $(X,d)$.
* If $F_{1},...,F_{n}$ are closed in $(X,d)$, then $\displaystyle\bigcup_{i=1}^{n} F_{i}$ is closed in $(X,d)$.
* If $\set{U_{i}:i\in\mathcal{I}}$ is any collection of sets that are open in $(X,d)$, where $\mathcal{I}$ is any index set, then $U = \displaystyle\bigcup_{i\in\mathcal{I}} U_{i}$ is open in $(X,d)$.
* If $\set{F_{i}: i\in\mathcal{I}}$ is any collection of closed sets in $(X,d)$ then $\displaystyle\bigcap_{i\in\mathcal{I}} F_{i}$ is closed in $(X,d)$.

### Convergence of sequences

#### Convergence

* A sequence $(x_{n})_{n=1}^{\infty} in $(X,d)$ converges to $x\in X$ if $$\lim_{n\to\infty} d(x_{n},x) = 0,$$ in terms of open balls this can be phrased as for every $\varepsilon > 0$ there exists $N\geq 1$ such that $$x_{n}\in\mathbb{B}(x,\varepsilon)$$ for all $n\geq N$.
* A subset $F$ of a metric space is closed if and only if whenever a sequence $(x_{n})_{n=1}^{\infty}$ contained in $F$ converges to some $x\in X$, it follows that $x\in F$.

### Continuity 

* Let $(X,d_{X})$ and $(Y,d_{Y})$ be metric spaces and let $f:X\to Y$ be a function. For $p\in X$, we say that $\displaystyle\lim_{x\to p}f(x) = y\in Y$ if for every $\varepsilon > 0$ there exists $\delta > 0$ such that $$0 < d_{X}(X, p) < \delta\implies d_{Y}(f(x),y) < \varepsilon. $$

* Let $(X, d_{X})$ and $(Y, d_{Y})$ be metric spaces and let $f: X\to Y$ be a function. Then $f$ is ***continuous*** at $p\in X$ if $\displaystyle\lim_{x\to p}f(x) = f(p)$, i.e. if for every $\varepsilon > 0$ there exists a $\delta > 0$ such that $$d_{X}(x, p) < \delta\implies d_{Y}(f(x), f(p)) < \varepsilon.$$
* It is ***continuous*** on $X$ if it is continuous at every point of $X$.

* A function $f:X\to Y$ is ***Lipschitz continuous*** or just ***Lipschitz*** if there exists $C\geq 0$ such that $$d_{Y}(f(x),f(y))\leq Cd_{X}(x,y)$$ for every $x,y\in X$.

* Let $(X,d_{X})$ and $(Y,d_{Y})$ be metric spaces. A function $f:X\to Y$ is continuous if and only if for any open set $U\subset Y, f^{-1}(U)$ is open in $X$.

### Topologically equivalence

Suppose that $d_{1}$ and $d_{2}$ are two metrics on $X$. Then the following statements are equivalent:

* every set that is open in $(X,d_{2})$ is open in $(X,d_{1})$;
* for any metric space $(Y,d_{Y})$, if $g:X\to Y$ is continuous from $(X,d_{2})$ into $(Y,d_{Y})$, then $g$ is continuous from $(X,d_{1})$ into $(Y,d_{Y})$ and 
* for any metric space $(Y,d_{Y})$, if $f:Y\to X$ is continuous from $(Y,d_{Y})$ into $(X,d_{1})$ then $f$ is continuous from $(Y,d_{Y})$ into $(X,d_{2})$.


Suppose that $d_{1}$ and $d_{2}$ are two metrics on $X$. Then the following statements are equivalent:

* the open sets in $(X,d_{1})$ and $(X,d_{2})$ coincide;
* for any metric space $(Y,d_{Y})$, a function $g:X\to Y$ is continuous from $(X,d_{1})$ into $(Y,d_{Y})$ if and only if $g$ is continuous from $(X,d_{2})$ into $(Y,d_{Y})$;
* for any metric space $(Y,d_{Y})$, a function $f:Y\to X$ is continuous from $(Y,d_{Y})$ into $(X,d_{1})$ if and only if $f$ is continuous from $(Y,d_{Y})$ into $(X,d_{2})$.

#### Topologically equivalent

* Two metrics $d_{1}$ and $d_{2}$ on $X$ are called ***topologically equivalent*** or just ***equivalent*** if the open setes in $(X,d_{1})$ and $(X,d_{2})$ coincide.
* Two metrics $d_{1}$ and $d_{2}$ on $X$ are called ***Lipschitz equivalent*** if there exists $0 < c\leq C < \infty$ such that $$cd_{1}(x,y)\leq d_{2}(x,y)\leq Cd_{1}(x,y)$$ for all $x,y\in X$.

#### Equivalent norms

* The metrics induced by equivalent norms are topologically equivalent.
* If $X$ is a vector space and two norms $\left\|\cdot\right\|_ {1}$ and $\left\|\cdot\right\|_ {2}$ on $X$ induce ***topologically equivalent metrics*** then the norms are equivalent.

### Isometries and homeomorphisms

* Suppose that $f:X\to Y$ is a bijection such that $$d_{Y}(f(x),f(y)) = d_{X}(x,y)$$ for all $x,y\in X$. Then $f$ is called an ***isometry*** between $X$ and $Y$. It preserves the distance between points, so $X$ and $Y$ are the same as metric spaces. We say that $X$ and $Y$ are ***isometric***.

* If $f:X\to Y$ is a bijection and both $f$ and $f^{-1}$ are continuous, we say that $f$ is a homeomorphism and that $X$ and $Y$ are ***homeomorphic***.

### Topological properties I

If some property $P$ of a metric space is such that if $(X,d)$ has property $P$, then so does every metric space that is homeomorphic to $(X,d)$ we say that $P$ is a ***topological property***.

Examples of topological properties:

* $X$ is open in $X$; $X$ is closed in $X$.
* $X$ is finite; countably infinite or uncountable.
* Every continuous real-valued function on $X$ is bounded.

Examples of properties that are not topological:

* $X$ is bounded.
* $X$ is totally bounded: for each $r > 0$ there exists a finite set  $F$ such that every ball of radius $r$ contains a point of $F$.

### Topological Spaces

#### Definition of a topology

A ***topology*** $\mathcal{T}$ on a set $T$ is a collection of subsets of $T$, which we agree to call the "open sets", such that 
* $T$ and $emptyset$ are open;
* the intersection of finitely many open sets is open; and
* arbitrary unions of open sets are open.

The pair $(T,\mathcal{T})$ is called a ***topological space***.

#### Definition of finer and coarser

* If $\mathcal{T}_ {1}$ and $\mathcal{T}_ {2}$ are two topologies on $T$ then we say that $\mathcal{T}_ {1}$ is ***coarser*** than $\mathcal{T}_ {2}$ if $\mathcal{T}_ {1}\subset \mathcal{T}_ {2}$, i.e. $\mathcal{T}_ {1}$ contains "fewer" open sets than $\mathcal{T}_ {2}$. In this situation, we also say that $\mathcal{T}_ {2}$ is ***finer*** than $\mathcal{T}_ {1}$. 

#### Closed topological space

A subset of a topological space $T$ is closed if its complement is open. Using De Morgan's laws, the collection $\mathcal{F}$ of all closed sets satisfies 

* $T$ and $\emptyset$ are closed.
* the union of finitely many closed sets is closed; and
* arbitrary intersections of closed sets are closed.

### Bases and sub-bases

A ***basis*** for a topology $\mathcal{T}$ on $T$ is a collection $\mathcal{B}\subset\mathcal{T}$ such that every set in $\mathcal{T}$ is the union of some sets from $\mathcal{B}$, i.e. for all $U\in\mathcal{T}$, there exists $\mathcal{C}_ {U}\subset\mathcal{B}$ such that $U = \displaystyle\bigcup_{\mathbb{B}\in\mathcal{C} _{U}}\mathbb{B}$.

If $\mathcal{B}$ is any basis for $\mathcal{T}$, then 

* $T$ is the union of some sets from $\mathcal{B}$ (i.e. there exists $\mathcal{C}_ {T}\subset\mathcal{B}$ such that \displaystyle\bigcup_{\mathbb{B}\in\mathcal{C}_ {T}}\mathbb{B} = T);
* If $\mathbb{B}_ {1},\mathbb{B}_ {2}\in\mathcal{B}$, then $\mathbb{B}_ {1}\cap\mathbb{B}_ {2}$ is the union of some sets from $\mathcal{B}$ (i.e. there exists $\mathcal{C}_ {\mathbb{B}_ {1}\cap\mathbb{B}_ {2}}\subset\mathcal{B}$ such that $\displaystyle\bigcup_{\mathbb{B}\in\mathcal{C}_ {\mathbb{B}_ {1}\cap\mathbb{B}_ {2}}}\mathbb{B} = \mathbb{B}_ {1}\cap\mathbb{B}_ {2}$.
