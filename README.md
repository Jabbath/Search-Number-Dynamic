# Dynamic Search Number

This is a networkx package that finds the mixed edge search number or edge search number of a graph. The package takes a dynamic programming approach to the
problem LINEAR-WIDTH, which can be related to searching by the techniques presented in "Computing Small Search Numbers in Linear Time" by Bodlaender et. al. 
This program runs in O(m!), where m is the numer of edges. 
However, in practice the algorithm tends to terminate quickly for some graphs with less than 20 edges.

## Usage

First, you must have a connected graph for input. Then, you can calculate the 
mixed edge search number or edge search number by the following:

```
import networkx as nx
from dynamic_search_number.mixedSearch import ms
from dynamic_search_number.edgeSearch import es

G = nx.cycle_graph(4)

print ms(G)
#2

print es(G)
#2
```

## License

See license.txt.

## Contribution

Contributions that improve performance or add functionality are welcome. Feel
free to submit a pull request.
