# transitive-closure
Alternate method of finding the transitive closure of graph or relation.

## What Is
The union of $`G^{k}`$ for all $`k\ge 1`$ (denoted $`G^{+}`$ represents reachability by walks of any positive length in G.
In taking the union of graphs, there is only one copy of the vertex set and the union is taken over the edge sets of the 
respective graphs.  **Remember, a digraph consists of (V, E) where V is set of vertices and E is set of edges.**

(u,v) is an edge in $`G^{+}`$ if vertex v can be reached from vertex u in G by a walk of any length.  If the vertex set is finite,
then only graph powers up to |V| are required.  Let G be a graph on a finite vertex set with n vertices.  Then:
$`G^{+} = G^{1}\cup G^{2}\cup ...\cup G^{n}`$
