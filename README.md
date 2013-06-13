AAIL-Art
========

*Abstract Art Involving Lines (AAIL)*

Create art using computer science.
This will initially be line diagrams using the Travelling Salesman Problem (TSP).

For the initial version, only Prim's algorithm is used.
Whilst this results in a Minimum Spanning Tree (MST) and not a TSP, the resulting images can still be pleasing.
This implementation of Prim's algorithm is also `O(n^2)` and will not scale well for large inputs.
For tuning, use the `simplify` command line option.

    Usage: aail [options] input_image output_image
    
    Options:
      -h, --help   show this help message and exit
      -n SIMPLIFY  Simplification amount (retain 1/n vertices for MST)

![](https://github.com/smerity/aail-art/raw/master/sample.png)
