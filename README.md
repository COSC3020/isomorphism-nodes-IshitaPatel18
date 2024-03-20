[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/AtNXzL3S)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Proof: Suppose $G_1$ consists of the vertices A, B, and C and $G_2$
consists of the vertices 1, 2, 3, and 4, where B shares an edge with C and
2 shares an edge with 3. So $G_1$ has 3 nodes and $G_4$ has 4 nodes, which means
they do not have the same number of nodes. Now suppose there is a function 
that maps the vertices of $G_1$ onto $G_2$ such that f(A) = 1, f(B) = 2, f(C) = 3.
The mapping of $G_1$ to $G_2$ shows that the vertex 4 in $G_2$ is not the 
image of a vertex in $G_1$, which makes the function not onto. If the function
that maps $G_1$ onto $G_2$ is not onto then the funtion is not the bijection
function required for $G_1$ to be isomorphic to $G_2$ because a bijection function
is one-to-one and onto. Therefore, if two graphs do not have the same number
of nodes, they cannot be isomorphic.

Sources: The Introduction to Algorithms textbook, pages 1161, 1162, and 1166
