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

Proof: For $G_1$ and $G_2$ to be isomorphic, there must exist a bijection function, 
which means a one-to-one and onto function exists. For a one-to-one function to exist, 
distinct vertices from $G_1$ must map to distinct vertices in $G_2$ (in this context).
For example, one vertex in $G_2$ can not be the image of 2 vertices in $G_1$. For a 
onto function to exist, it must be possible to map all vertices in $G_2$ to a vertex 
in $G_1$ (in this context). A bijection leads to a one-to-one correspondence or essentially 
a pairing of vertices in this case. Now lets say $G_1$ has any number of vertices 
and $G_2$ has any number of vertices less than $G_1$. So $G_1$ will have more 
vertices than $G_2$. Now if we want our pairing of vertices to occur, 
we start mapping one vertex from $G_1$ onto a vertex in $G_2$. As we continue
mapping, $G_2$ will run out of vertices first as it has fewer vertices than $G_1$. 
So, $G_1$ must map it's remaining vertices to a non unique vertex in $G_2$ to allow
a function to exists, but it means the function is no longer one-to-one as more than
one vertex in $G_1$ is mapped to the same vertex in $G_2$. Now, lets say that $G_2$
has any number of vertices and $G_1$ has any number of vertices less than $G_2$, so 
$G_2$ has more vertices than $G_1$. Now as we map the vertices of $G_1$ onto the vertices
of $G_2$ creating pairings as we go, we would find that $G_1$ runs out of vertices to pair
with $G_2$ meaning not all the vertices in $G_2$ would have an image of a vertex in $G_1$
under the function, so the function that maps $G_1$ onto $G_2$ would not be onto. If we chose
to map the remaining vertices of $G_2$ then our function would be onto, but no longer one-to-one.
Therefore, we see that not having the same number of nodes leads to a function that is either onto or
one-to-one, but not both which is required for a bijection function that allows $G_1$ to be
isomorphic to $G_2$, so if both graphs do not have the same number of nodes, they can not
be isomorphic as a bijection is not achievable.

Sources: The Introduction to Algorithms textbook, pages 1161, 1162, and 1166
https://en.wikipedia.org/wiki/Bijection,_injection_and_surjection#:~:text=The%20function%20is%20injective%2C%20or,distinct%20elements%20in%20the%20codomain.
https://www.geeksforgeeks.org/injective-functions/

