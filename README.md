# cubes.ipynb
* Represent the state of the elements as a float tensor (np array)
* Represent the graph of neighbors as a row-normalized adjacency matrix, where each row represents a probability distribution over the neighbors of the given node. 
  * See helper function `get_normalized_undirected_adjacency()`
## Usage
* `steps()` is a convenience wrapper that runs the process for N steps
* `steps()` takes as an argument a function that runs a single step (example: `step_with_confidence()`)
## Analysis
* Plot statistics for each step over time - `summarize_by_step()`
  * [WIP] analytically estimate stable state (stationary distribution) by computing leading eigenvector of adjacency matrix (See Ferron-Frobenius Theorem)
## Dependencies
* numpy, scipy, pandas, networkx