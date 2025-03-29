# transitive-closure
Alternate method of finding the transitive closure of graph or relation.

## What Is
The union of $`G^{k}`$ for all $`k\ge 1`$ (denoted $`G^{+}`$ represents reachability by walks of any positive length in G.
In taking the union of graphs, there is only one copy of the vertex set and the union is taken over the edge sets of the 
respective graphs.  **Remember, a digraph consists of (V, E) where V is set of vertices and E is set of edges.**

(u,v) is an edge in $`G^{+}`$ if vertex v can be reached from vertex u in G by a walk of any length.  If the vertex set is finite,
then only graph powers up to |V| are required.  Let G be a graph on a finite vertex set with n vertices.  Then:

$`G^{+} = G^{1}\cup G^{2}\cup ...\cup G^{n}`$

The same definition holds for a relation R.
The relation $`R^{+}`$ is the TRANSITIVE CLOSURE OF R and is the smallest relation that is both transitive and includes  
all the pairs from R.  In other words, any relation that contains all the pairs from R and is transitive must include all
the pairs in $`R^{+}`$.  The same applies for directed graph G.

## Direct Method
Graph each power of G (up to $`G^{k}`$) and combine every edge into $`G^{+}`$

## Alternate Method
There is another way to find the transitive closure of a graph or relation that does not require computing the powers directly.
The process repeatedly looks for three elements x, y, z, such that (x,y) and (y,z) are pairs in the relation but (x,z)
is not in the relation.  If there is such a triplet of elements, then the pair (x,z) is added to the relation.  The process
ends when there is no such triplet of elements.

Repeat the following step until no pair is added to R.
  If there are three elements x,y,z ∈ A such that (x,y) ∈ R, (y,z) ∈ R and (x,z) ∉ R, then add (x,z) to R
