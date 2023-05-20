# MA260-Norms-Metrics-and-Topologies-Revision
My own notes about the MA260 Norms, Metrics and Topologies revision, mainly from the notes and example sheets.


- [MA260-Norms-Metrics-and-Topologies-Revision](#ma260-norms-metrics-and-topologies-revision)
  * [Lecture notes](#lecture-notes)
  * [Example sheets](#example-sheets)
    + [Countable](#countable)
    + [Norms](#norms)
      - [Standard norm/Euclidean norm](#standard-norm-euclidean-norm)
      - [Normed space](#normed-space)
      - [Closed unit ball](#closed-unit-ball)
      - [Convex](#convex)
      - [Minkowski's inequality in $\mathbb{R}^{n}$](#minkowski-s-inequality-in---mathbb-r---n--)
        * [Equivalent norms](#equivalent-norms)
      - [$l^{p}$ space](#-l--p---space)
      - [Minkowski's inequality in $l^{p}$](#minkowski-s-inequality-in--l--p--)
      - [$L^{p}$ space](#-l--p---space)
    + [Metric space](#metric-space)
      - [Standard metric/Euclidean metric](#standard-metric-euclidean-metric)
      - [Discrete metric](#discrete-metric)
      - [Sunflower metric](#sunflower-metric)
      - [Jungle river metric](#jungle-river-metric)
    + [Open and closed sets](#open-and-closed-sets)
      - [Bounded subsets](#bounded-subsets)
      - [Open and closed subsets](#open-and-closed-subsets)
    + [Convergence of sequences](#convergence-of-sequences)
      - [Convergence](#convergence)
    + [Continuity](#continuity)
      - [Continuity and open/close sets](#continuity-and-open-close-sets)
    + [Topologically equivalence](#topologically-equivalence)
      - [Topologically equivalent](#topologically-equivalent)
      - [Equivalent norms](#equivalent-norms-1)
    + [Isometries and homeomorphisms](#isometries-and-homeomorphisms)
    + [Topological properties I](#topological-properties-i)
    + [Topological Spaces](#topological-spaces)
      - [Definition of a topology](#definition-of-a-topology)
      - [Definition of finer and coarser](#definition-of-finer-and-coarser)
      - [Closed topological space](#closed-topological-space)
    + [Bases and sub-bases](#bases-and-sub-bases)
    + [Subspaces and finite product spaces](#subspaces-and-finite-product-spaces)
      - [Subspace topology](#subspace-topology)
      - [Product topological spaces](#product-topological-spaces)
    + [Closure, interior and boundary](#closure--interior-and-boundary)
      - [Closure](#closure)
      - [Interior](#interior)
      - [Relationship between closure and interior](#relationship-between-closure-and-interior)
      - [Boundary](#boundary)
      - [Limit point and Isolated point](#limit-point-and-isolated-point)
      - [Dense, nowhere dense and meagre](#dense--nowhere-dense-and-meagre)
    + [The Hausdorff property and metrisability](#the-hausdorff-property-and-metrisability)
    + [Continuity between topological spaces](#continuity-between-topological-spaces)
    + [Basic properties](#basic-properties)
      - [Transitivity of continuity](#transitivity-of-continuity)
      - [Projection continuity](#projection-continuity)
      - [Additivity, product and division continuity](#additivity--product-and-division-continuity)
    + [The projective topology and product spaces](#the-projective-topology-and-product-spaces)
    + [Homeomorphisms](#homeomorphisms)
    + [Compactness](#compactness)
      - [Cover and subcover](#cover-and-subcover)
      - [Compact](#compact)
      - [Heine-Borel Theorem](#heine-borel-theorem)
    + [Compact vs closed](#compact-vs-closed)
    + [Compactness of products and compact subsets of $\mathbb{R}^{n}$](#compactness-of-products-and-compact-subsets-of---mathbb-r---n--)
      - [Tychonov's Theorem](#tychonov-s-theorem)
      - [Heine-Borel in $\mathbb{R}^{n}$](#heine-borel-in---mathbb-r---n--)
    + [Continuous functions on compact sets](#continuous-functions-on-compact-sets)
      - [Semicontinuous](#semicontinuous)
    + [Equivalence of all norms on $\mathbb{R}^{n}$](#equivalence-of-all-norms-on---mathbb-r---n--)
    + [Lebesgue numbers and uniform continuity](#lebesgue-numbers-and-uniform-continuity)
      - [Uniformly continuous](#uniformly-continuous)
    + [Sequential compactness](#sequential-compactness)
    + [Normed spaces](#normed-spaces)
    + [Connectedness](#connectedness)
      - [Connected/Disconnected](#connected-disconnected)
      - [Subset connected/disconnected](#subset-connected-disconnected)
    + [Connected subsets of $\mathbb{R}$](#connected-subsets-of---mathbb-r--)
    + [Operations on connected sets](#operations-on-connected-sets)
      - [Topologist sine curve](#topologist-sine-curve)
    + [Connected components](#connected-components)
    + [Path-connected spaces](#path-connected-spaces)
    + [Open sets in $\mathbb{R}^{n}$](#open-sets-in---mathbb-r---n--)
      - [Cauchy sequence](#cauchy-sequence)
    + [Completeness](#completeness)
      - [Examples of complete spaces](#examples-of-complete-spaces)
    + [Completions](#completions)



## Lecture notes

[260_notes_2022-23.pdf](https://github.com/Louisli0515/MA260-Norms-Metrics-and-Topologies-Revision/files/11422967/260_notes_2022-23.pdf)

First of all, feel free to download 2022-2023 lecture notes for MA260.

## Example sheets

[MA260_Norms_metrics_topologies_tutorial_sheet.pdf](https://github.com/Louisli0515/MA260-Norms-Metrics-and-Topologies-Revision/files/11456167/MA260_Norms_metrics_topologies_tutorial_sheet.pdf)

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

* A sequence $(x_{n})_ {n=1}^{\infty}$ in $(X,d)$ converges to $x\in X$ if $$\lim_{n\to\infty} d(x_{n},x) = 0,$$ in terms of open balls this can be phrased as for every $\varepsilon > 0$ there exists $N\geq 1$ such that $$x_{n}\in\mathbb{B}(x,\varepsilon)$$ for all $n\geq N$.
* A subset $F$ of a metric space is closed if and only if whenever a sequence $(x_{n})_{n=1}^{\infty}$ contained in $F$ converges to some $x\in X$, it follows that $x\in F$.

### Continuity 

* Let $(X,d_{X})$ and $(Y,d_{Y})$ be metric spaces and let $f:X\to Y$ be a function. For $p\in X$, we say that $\displaystyle\lim_{x\to p}f(x) = y\in Y$ if for every $\varepsilon > 0$ there exists $\delta > 0$ such that $$0 < d_{X}(X, p) < \delta\implies d_{Y}(f(x),y) < \varepsilon. $$

* Let $(X, d_{X})$ and $(Y, d_{Y})$ be metric spaces and let $f: X\to Y$ be a function. Then $f$ is ***continuous*** at $p\in X$ if $\displaystyle\lim_{x\to p}f(x) = f(p)$, i.e. if for every $\varepsilon > 0$ there exists a $\delta > 0$ such that $$d_{X}(x, p) < \delta\implies d_{Y}(f(x), f(p)) < \varepsilon.$$
* It is ***continuous*** on $X$ if it is continuous at every point of $X$.

* A function $f:X\to Y$ is ***Lipschitz continuous*** or just ***Lipschitz*** if there exists $C\geq 0$ such that $$d_{Y}(f(x),f(y))\leq Cd_{X}(x,y)$$ for every $x,y\in X$.

* Let $(X,d_{X})$ and $(Y,d_{Y})$ be metric spaces. A function $f:X\to Y$ is continuous if and only if for any open set $U\subset Y, f^{-1}(U)$ is open in $X$.

#### Continuity and open/close sets

* If $f:\mathbb{R}^{n}\to\mathbb{R}^{k}$ is continuous at all points of $\mathbb{R}^{n}$, then for all open subsets $V$ of $\mathbb{R}^{k}$, $f^{-1}(V)$ is open; for all closed subsets $\mathcal{F}$ of $\mathbb{R}^{k}$, $f^{-1}(\mathcal{F})$ is closed.

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

* A ***basis*** for a topology $\mathcal{T}$ on $T$ is a collection $\mathcal{B}\subset\mathcal{T}$ such that every set in $\mathcal{T}$ is the union of some sets from $\mathcal{B}$, i.e. for all $U\in\mathcal{T}$, there exists $\mathcal{C}_ {U}\subset\mathcal{B}$ such that $U = \displaystyle\bigcup_{B\in\mathcal{C} _ {U}}B$.

If $\mathcal{B}$ is any basis for $\mathcal{T}$, then 

* $T$ is the union of some sets from $\mathcal{B}$ (i.e. there exists $\mathcal{C}_ {T}\subset\mathcal{B}$ such that $\displaystyle\bigcup_{B\in\mathcal{C}_ {T}} B = T)$;
* If $B_{1},B_{2}\in\mathcal{B}$, then $B_{1}\cap B_{2}$ is the union of some sets from $\mathcal{B}$ (i.e. there exists $\mathcal{C}_ {B_{1}\cap B_{2}}\subset\mathcal{B}$ such that $\displaystyle\bigcup_{B\in\mathcal{C}_ {B_{1}\cap B_{2}}}B = B_{1}\cap B_{2}$.

* A ***sub-basis*** for a topology $\mathcal{T}$ on $T$ is a collection $\mathcal{B}\subset\mathcal{T}$ such that every set in $\mathcal{T}$ is a union of finite intersections of sets from $\mathcal{B}$.

### Subspaces and finite product spaces

#### Subspace topology

* If $(T,\mathcal{T})$ is a topological space and $S\subset T$, then the ***subspace topology*** on $S$ is $$\mathcal{T}_ {S} = \set{U\cap S:U\in\mathcal{T}}.$$ We call $(S,\mathcal{T}_ {S})$ a topological subspace of $T$.

#### Product topological spaces

* Suppose that $(T_{1},\mathcal{T}_ {1})$ and $(T_{2}, \mathcal{T}_ {2})$ are two topological spaces. Then the ***product topology*** on $T_{1}\times T_{2}$ is the topology $\mathcal{T}$ with basis $$\mathcal{B} = \set{U_{1}\times U_{2}: U_{1}\in\mathcal{T}_ {1}, U_{2}\in\mathcal{T}_ {2}}.$$ We call $(T_{1}\times T_{2}, \mathcal{T})$ the topological product of $T_{1}$ and $T_{2}$.

### Closure, interior and boundary

* A neighbourhood of $x\in T$ is a set $H\subset T$ such that $x\in U\subset H$ for some $U\in\mathcal{T}$. An ***open neighbourhood*** of $x\in T$ is an open set $U$ that contains $x$.

#### Closure

* The ***closure*** $\overline{A}$ of a set $A\subset T$ is the intersection of all closed sets that contain $A$.
* The closure of $A$, $\overline{A}$ is the set $$\overline{A} = \set{x\in T:U\cap A\ne\emptyset\text{for every open set U that contains x}} = \set{x\in T:\text{every neighbourhood of x intersects A}}.$$
* If $X$ is a metric space and $A\subset X$ then $$\overline{A} = \set{\text{limits of convergent sequences in A}}.$$

#### Interior

* The ***interior*** of $A$, $A^{\circ}$, is the union of all open subsets of $A$.
* The interior of $A$, $A^{\circ}$ consists of all points for which $A$ is a neighbourhood, i.e. $$\set{x\in T:x\in U\subset A\, \text{for some} U\in\mathcal{T}}.$$

#### Relationship between closure and interior

* If $A\subset T$, then $$A^{\circ} = T\setminus\overline{T\setminus A}\quad\text{and}\quad\overline{A} = T\setminus(T\setminus A)^{\circ}.$$

#### Boundary

* The boundary $\partial H$ of a set $H$ is the set of all points $x$ whith the property that every neighbourhood of $x$ meets both $H$ and its complement: $$\partial H = \set{x\in T: \text{if U is an open set that contains x then} U\cap H\ne\emptyset\, U\cap(T\setminus H)\ne\emptyset}.$$
* We have $$\partial H = \overline{H}\setminus H^{\circ}.$$

#### Limit point and Isolated point

* Let $S\subset T$. A point $x\in T$ is a ***limit point*** of $S$ if every neighbourhood of $x$ intersects $S\setminus\set{x}$.
* A point in $S$ that is not a limit point of $S$ is called an ***isolated point***.

#### Dense, nowhere dense and meagre

A subset $A$ of $T$ is 

* ***dense*** in $T$ if $\overline{A} = T$;
* ***nowhere dense*** in $T$ if $(\overline{A})^{\circ} = \emptyset$;
* ***meagre*** in $T$ if it is a union of a countable number of nowhere dense sets.

### The Hausdorff property and metrisability

* A topological space $(T,\mathcal{T})$ is ***metrisable*** if there is a metric $d$ on $T$ such that $\mathcal{T}$ consists of the open sets in $(T,d)$.
* A sequence $(x_{n})^{\infty}_ {n=1}$ in a topological space $T$ converges to $x$ if for every open neighbourhood $U$ of $x$ there exists $N\geq 1$ such that $x_{n}\in U$ for all $n\geq N$.
* A topological space $T$ is ***Hausdorff*** if for any two distinct $x,y\in T$, there exist disjoint open sets $U,V$ such that $x\in U$ and $y\in V$.
* In a Hausdorff space $T$, any sequence has ***at most*** one limit.

### Continuity between topological spaces

* A map $f:T_{1}\to T_{2}$ between two topological spaces $(T,\mathcal{T}_ {1})$ and $(T_{2},\mathcal{T}_ {2})$ is ***continuous*** if whenever $U\subset T_{2}$ is open, $f^{-1}(U)$ is open in $T_{1}$. (i.e. if $U\in\mathcal{T}_ {2}$, then $f^{-1}(U)\in\mathcal{T}_ {1}$).
* Suppose that $f:T_{1}\to T_{2}$ is a map between two topological spaces $(T_{1},\mathcal{T}_ {1})$ and $(T_{2},\mathcal{T}_ {2})$, and that $\mathcal{B}$ is a sub-basis for the topology $\mathcal{T}_ {2}$. Then $f$ is ***continuous*** if and only if $f^{-1}(B)$ is open in $T_{1}$ for every $B\in\mathcal{B}$.

### Basic properties

#### Transitivity of continuity

* If $(T_{1}, \mathcal{T}_ {1})$, $(T_{2},\mathcal{T}_ {2})$ and $(T_{3}, \mathcal{T}_ {3})$ are topological spaces and $f: T_{1}\to T_{2}$ and $g: T_{2}\to T_{3}$ are ***continuous***, then $g\circ f: T_{1}\to T_{3}$ is ***continuous***.

#### Projection continuity

* For $j = 1,2$, the projection $\pi_{j}: T_{1}\times T_{2}\to T_{j}$ is ***continuous***.
* Let $(T,\mathcal{T}), (T_{1},\mathcal{T}_ {1})$ and $(T_{2},\mathcal{T}_ {2})$ be topological spaces. A map $f = (f_{1},f_{2}):T\to T_{1}\times T_{2}$ is ***continuous*** if and only if $f_{1}$ and $f_{2}$ are ***both continuous***. (i.e. $\pi_{1}\circ f$ and $\pi_{2}\circ f$ are continuous).

#### Additivity, product and division continuity

* If $f,g:T\to\mathbb{R}$ are ***continuous***, then so are $f+g, fg$ and $f/g$ is ***continuous*** on the set $\set{x\in T: g(x)\ne 0}$.

### The projective topology and product spaces

* The ***projective topology*** on $T$ is the coarsest topology for which all the maps $f_{j}:T\to T_{j}$ are continuous.
* Let $(T_{j},\mathcal{T}_ {j}), j\in J$ be an arbitrary collection of topological spaces. Their product $T = \displaystyle\prod_{j\in J} T_{j}$ is the set of all functions $x:J\to\displaystyle\bigcup_{j\in J} T_{j}$ such that $x(j)\in T_{j}$. The product topology $\mathcal{T}$ on $T$ is the coarsest topology for which all of the projections $$\pi_{j}: T\to T_{j}:x\mapsto x(j)$$ are continuous. We then call the topological space $(T,\mathcal{T})$ the topological product of the spaces $(T_{j},\mathcal{T}_ {j})$.
* A sub-basis for the product topology consists of all sets of the form $$\prod_{j\in J} U_{j},$$ where $U_{j}\in\mathcal{T}_ {j}$ with $U_{j} = T_{j}$ except for a finite number of the $j$.

### Homeomorphisms

Let $(T_{1},\mathcal{T}_ {1})$ and $(T_{2}, \mathcal{T}_ {2})$ be topological spaces. A bijection $f: T_{1}\to T_{2}$ is a ***homeomorhpism*** if any one of the following equivalent conditions holds:

* both $f$ and $f^{-1}$ are continuous;
* $V$ is open in $T_{2}$ if and only if $f^{-1}(V)$ is open in $T_{1}$.
* $U$ is open in $T_{1}$ if and only if $f(U)$ is open in $T_{2}$.

If there is a homemorphism $f:T_{1}\to T_{2}$, we say that $(T_{1},\mathcal{T}_ {1})$ and $(T_{2},\mathcal{T}_ {2})$ are ***homeomorphic***.

* A property of topological spaces is a ***topological invariant*** (or 'topological property') if it is preserved by homeomorphisms.

### Compactness

#### Cover and subcover

* A ***cover*** of a set $A$ is collection $\mathcal{U}$ of sets whose union contains $A$: $$A\subset\bigcup_{U\in\mathcal{U}} U.$$
* A ***subcover*** of a cover $\mathcal{U}$ is a subset of $\mathcal{U}$ whose elements still cover $A$. 
* A cover is ***open*** if all of its elements are open.

#### Compact

* A topological space $T$ is ***compact*** if every open cover of $T$ has a finite subcover.
* A subset $S$ of $T$ is ***compact*** if every open cover of $S$ by subsets of $T$ has a finite subcover. This is the same as $S$ being compact with the subspace topology.
* If $T$ is a topological space and $S\subset T$, then $S$ is ***compact*** in the sense of definition of compact if and only if $(S,\mathcal{T}_ {S})$ is compact in the sense of definition of compact.

#### Heine-Borel Theorem

* Any closed interval $[a,b]$ is a ***compact subset*** of $\mathbb{R}$ (with the usual topology).

### Compact vs closed

* Any ***closed subset*** $S$ of a ***compact space*** $T$ is compact.
* Any ***compact subset*** $K$ of a ***Hausdorff space*** $T$ is closed.
* Any ***compact subset*** $K$ of a metric space $(X,d)$ is ***bounded***.
* A subset of $\mathbb{R}$ with the usual topology is ***compact*** if and only if it is ***closed and bounded***.
* Let $\mathcal{F}$ be a collection of non-empty closed subsets of a compact space $T$ such that every finite subcollection of $\mathcal{F}$ has a non-empty intersection. Then the intersection of all the sets from $\mathcal{F}$ is non-empty.
* Let $F_{1}\supset F_{2}\supset F_{3}\supset...$ be non-empty closed subsets of a compact space $T$. Then $\displaystyle\bigcap_{j=1}^{\infty} F_{j}\ne\emptyset.$

### Compactness of products and compact subsets of $\mathbb{R}^{n}$

* If $T$ and $S$ are compact topological spaces, then $T\times S$ is compact.
* The product of a finite numnber of compact spaces is compact.

#### Tychonov's Theorem

* The product of any collection of compact spaces is compact (with the product topology).

#### Heine-Borel in $\mathbb{R}^{n}$

* A subset of $\mathbb{R}^{n}$ is ***compact*** if and only if it is closed and bounded.

### Continuous functions on compact sets

* A ***continuous*** image of a compact space is compact.
* A ***continuous bijection*** of a compact space $T$ onto a Hausdorff space $S$ is a homeomorphism.

#### Semicontinuous

* A function $f:T\to\mathbb{R}$ is ***lower semicontinuous*** if for every $c\in\mathbb{R}$, the set $f^{-1}(c,\infty)$ is open.
* It is ***upper semicontinuous*** if for every $c\in\mathbb{R}$, the set $f^{-1}(-\infty.c)$ is open.
* If $f:T\to\mathbb{R}$ is both ***upper and lower semicontinuous***, then $$f^{-1}(a,\infty)\cap f^{-1}(-\infty,b) = f^{-1}(a,b)$$ is open for every $a,b\in\mathbb{R}$, and so $f$ is continuous.
* If $T$ is non-empty and compact and $f:T\to\mathbb{R}$ is ***lower semicontinuous*** then it is bounded below and attains its minimum.
* If $f$ is upper semicontinuous, then it is bounded above and attains its maximum.
* If $T$ is non-empty and compact, then a continuous function $f:T\to\mathbb{R}$ is ***bounded*** and ***attains its bounds***.

### Equivalence of all norms on $\mathbb{R}^{n}$

* All norms on $\mathbb{R}^{n}$ are equivalent.

### Lebesgue numbers and uniform continuity

* Let $\mathcal{U}$ be an open cover of a metric space $(X,d)$. A number $\delta > 0$ is called a ***Lebesgue number*** for $\mathcal{U}$ if for any $x\in X$, there exists $U\in\mathcal{U}$ such that $\mathbb{B}(x,\delta)\subset U$.
* Every open cover $\mathcal{U}$ of a compact metric space $(X,d)$ has a ***Lebesgue number***.

#### Uniformly continuous

* A map $f:(X,d_{X})\to (Y, d_{Y}) is ***uniformly continuous*** if for every $\varepsilon > 0$, there exists $\delta > 0$ such that $$d_{X}(x,y) < \delta \implies d_{Y}(f(x),f(y)) < \varepsilon$$ for any $x,y\in X$.
* A continuous map from a compact metric space into a metric space is uniformly continuous.

### Sequential compactness

* A subset $K$ of a metric space $(X,d)$ is ***sequentially compact*** if every sequence in $K$ has a convergent subsequence whose limit lies in $K$.
* If $K$ is a sequentially compact subset of a metric space, then any open cover of $K$ has a ***Lebesgue number***.
* A subset of a metric space is ***sequentially compact*** if and only if it is compact.

### Normed spaces

* A ***normed space*** is ***finite-dimensional*** if and only if its closed unit ball is compact.

### Connectedness

* We say that a pair of sets $(A,B)$ is a partition of a topological space $T$ if $T = A\cup B$ and $A\cap B = \emptyset$; and we then say that $A$ and $B$ partition $T$.

#### Connected/Disconnected

* A topological space $T$ is ***connected*** if the only partitions of $T$ into open sets are $(T,\emptyset)$ and $(\emptyset, T)$. The space $T$ is said to be ***disconected*** if it is not connected.

The following are equivalent:

* $T$ is disconnected;
* $T$ has a partition into two ***non-empty*** open sets.
* $T$ has a partition into two ***non-empty*** closed sets.
* $T$ has a subset that is both open and closed and is neither $\emptyset$ nor $T$.
* There is a continuous function from $T$ onto the two-point set $\set{0,1}$ with the ***discrete topology***.

#### Subset connected/disconnected

* A subset $S$ of $T$ is ***connected/disconnected*** if $(S,\mathcal{T}_ {S})$ is ***connected/disconnected***.
* A set $S\subset T$ is separated by subsets $U,V\in\mathcal{T}$ if $$S\subset U\cup V,\quad U\cap V\cap S = \emptyset,\quad U\cap S\ne\emptyset,\quad V\cap S\ne\emptyset.$$
* A subspace $S$ of a topological space $T$ is ***disconnected*** if and only if it is separated by some open subsets $U,V\in\mathcal{T}.$

### Connected subsets of $\mathbb{R}$

* A set $I\subset\mathbb{R}$ is an ***interval*** if and only if whenever $x,y\in I$ and $x < z < y$, we have $z\in I$.
* A subset of $\mathbb{R}$ is ***connected*** if and only if it is an interval.

### Operations on connected sets

* Suppose that $C_{j}, j\in\mathcal{J}$, are ***connected subsets*** of $T$ and $C_{i}\cap C_{j}\ne\emptyset$ for each $i,j$, then $$K = \bigcup_{j\in\mathcal{J}} C_{j}$$ is ***connected***.
* Suppose that $C_{1}$ and $C_{2}$ are ***connected subsets*** of $T$ and $\overline{C}_ {1}\cap C_{2}\ne\emptyset$. Then $C_{1}\cup C_{2}$ is ***connected***.
* If $C\subset T$ is ***connected***, then so is any set $K$ satisfying $C\subset K\subset\overline{C}$.
* The ***continuous image*** of a ***connected set*** is connected.
* The ***product*** of two ***connected spaces*** is ***connected***.

#### Topologist sine curve

* The 'topologist's sine curve' is given by $$\mathcal{F} = \set{\left(x,\sin\frac{1}{x}\right):x\in\mathbb{R},x\ne 0}\cup\set{(0,0)}$$ and it is connected.

### Connected components

The equivalence class of $\sim$ are called the ***connected components*** of $T$.

### Path-connected spaces

* If $u,v\in T$, a ***path*** from $u$ to $v$ is a ***continuous*** map $\varphi:[0,1]\to T$ such that $\varphi(0) = u$ and $\varphi(1) = v$. 
* A space $T$ is ***path connected*** if any two points in $T$ can be joined by a path in $T$.
* A ***path-connected*** space $T$ is ***connected***.

### Open sets in $\mathbb{R}^{n}$

* ***Connected open subsets*** of $\mathbb{R}^{n}$ are ***path connected***.
* Open subsets of $\mathbb{R}^{n}$ have open connected components.
* A subset $U$ of $\mathbb{R}$ is ***open*** if and only if it is the ***disjoint union*** of countably many open intervals, i.e. $U = \displaystyle\bigcup_{j\in\mathcal{J}}(a_{j}, b_{j})$, with the intervals ***disjoint*** and $\mathcal{J}$ ***finite*** or ***countably infinite***.

#### Cauchy sequence

* If a sequence $(x_{n})$ converges in a metric space $(X,d)$, then it is Cauchy, i.e. for every $\varepsilon > 0$, there exists $N$ such that $$d(x_{n},x_{m}) < \varepsilon$$ for every $n,m\geq N$.

### Completeness

* A metric space $(X,d)$ is ***complete*** if any Cauchy sequence in $X$ converges.
* Suppose that $(X,d)$ is a metric space and that $S$ is a subset of $X$. If $(S,d|_ {S})$ is ***complete***, then $S$ is a ***closed subset*** of $X$, and if $(X,d)$ is ***complete*** and $S$ is ***closed***, then $(S,d|_ {S})$ is ***complete***.
* Any ***compact metric space*** $(X,d)$ is complete.

#### Examples of complete spaces

* $\mathbb{R}^{d}$ is complete.
* For every $1\leq p\leq\infty$, $l^{p}$ is ***complete***.
* For any non-empty set $X$, the space $B(X)$ of ***bounded real-valued*** functions on $X$, $f:X\to\mathbb{R}$, with the 'sup norm' $$\left\|f\right\|_ {\infty} = \sup_{x\in X}\left|f(x)\right|$$ is ***complete***.
* The space $C_{b}(T)$ of all ***bounded continuous functions*** from any non-empty topological space $T$ into $\mathbb{R}$ is a closed subspace of $B(T)$, and hence ***complete***.
* If $T$ is non-empty and ***compact***, then $C(T)$ is ***complete*** with the maximum norm $$\left|f\right|_ {\infty} = \max_{x\in T}\left|f(x)\right|.$$

### Completions

* Any metric space $(X,d)$ can be ***isometrically embedded*** into the complete metric space $B(X)$.
* Any metric space has a ***completion***.
