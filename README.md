[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12578349&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

# Response
Consider two completely connected graphs of the same size n, $G_A$ and $G_B$. For a completely connected graph, each node has an edge connecting it to each other node in the graph. Now, consider a function $f$ which starts with an arbitrary node in $G_A$ and maps it to an arbitrary node in $G_B$. The function $f$ then repeats this process for each node in $G_A$ which hasn't been mapped to a node in $G_B$, and no node in $G_B$ has two nodes from $G_A$ mapped to it. Since $G_A$ and $G_B$ have the same number of nodes n, $f$ is a bijective function, as it is both one-to-one and onto.

Now, since $G_A$ and $G_B$ are completely connected graphs, it follows that each edge in $G_A$ will correspond to an equivalent edge in $G_B$. Therefore, if two completely graphs are of the same size, they are isomorphic.