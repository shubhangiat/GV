# GV

The base folder contains binary for four algorithms, each in a separate folder.
The mapping with respect to the algorithm names in the paper to the corresponding code folder is given below.

* GV-(2,1): two_units
* GV-(3,1): three_units
* GV-(2,2): two_pair
* GV-(1,1): one_unit

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

## Example
A sample Barabási-Albert graph has been provided in the dataset folder along with some queries and the corresponding query file.

Following commands could be run from the base folder on the sample graph for various algorithms.

* GV-(2,1)
  - ```two_units/subgraph dataset/v1k_l50_labels dataset/v1k_m5_edges dataset/qry_files```
* GV-(3,1): three_units
  - ```three_units/subgraph dataset/v1k_l50_labels dataset/v1k_m5_edges dataset/qry_files```
* GV-(2,2): two_pair
  - ```two_pair/subgraph dataset/v1k_l50_labels dataset/v1k_m5_edges dataset/qry_files```
* GV-(1,1): one_unit
  - ```one_unit/subgraph dataset/v1k_l50_labels dataset/v1k_m5_edges dataset/qry_files```


