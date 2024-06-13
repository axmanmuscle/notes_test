
# Introduction
This will serve as a small refresher about some linear algebra topics that will be useful later. 

# Vectors
A vector, as we know, is a collection of elements that has a direction and a magnitude. The most common case for this is a vector in $\mathbb{R}^n$, the _n_-dimensional real vector space.

There are some things that can trip us up here. To be most precise, a vector space has an associate scalar field. There is a distinction between where our vectors come from and where our scalars come from. To illustrate, consider the space of two-dimensional complex vectors. We'll call it $\mathbb{C}^2$ for right now and let
$$x \in \mathbb{C}^2 \, \implies \, x = \begin{bmatrix} x_1 \\ x_2 \end{bmatrix}, \, x_i \in \mathbb{C}.$$

This seems straightforward and if I were to ask you what the dimension of this space is, you'd say "clearly it's dimension two." This is true if the scalar field is also complex. The basis in this case is
$$e_1 = \begin{bmatrix} 1 \\ 0 \end{bmatrix} , \qquad e_2 = \begin{bmatrix} 0 \\ 1 \end{bmatrix},$$
since we can form any $x \in \mathbb{C}^2$ from these two vectors. However if the scalar field is _real_, so we draw our scalars from $\mathbb{R}$, this vector space is now dimension four. The basis vectors are
$$e_1 = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \; e_2 = \begin{bmatrix} 0 \\ 1 \end{bmatrix}, \; e_3 = \begin{bmatrix} i \\ 0 \end{bmatrix}, \; e_4 = \begin{bmatrix} 0 \\ i \end{bmatrix},$$
where $i$ is defined as the usual imaginary unit $i^2 = -1$. Here we need four vectors to span the entire space since we do not have the luxury of complex scalars.

# Matrices
There are several interpretations of matrices that are useful at any given time. We start with the most straightforward -- matrices as linear transformations.
## Linear Transformations
Let $\mathcal{X}, \mathcal{Y}$ be real vector spaces of dimension $n_x, n_y$ respectively. A transformation $A : \mathcal{X} \to \mathcal{Y}$  is linear if