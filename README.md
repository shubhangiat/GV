# GraMaR

## Command
For each algorithm, to execute the binary file run the following command.

```./subgraph file1 file2 file3```

## Parameters
* file1: vertex label file
  - format: `vertex_id vertex_label`
* file2: edge file path
  - format: `vertex_id1 vertex_id2`
* file3: file containing paths of query graphs
  - format: `query_vertex_label_file query_edge_file`

Output is to stdout.
The output of each query graph is further processed and sorted based on their chi-squared value.

A sample Barabási-Albert graph has been provided in the dataset folder along with some queries and the corresponding query file.
