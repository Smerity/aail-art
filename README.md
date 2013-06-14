AAIL-Art
========

*Abstract Art Involving Lines (AAIL)*

Create art using computer science.
This will initially be line diagrams using the Travelling Salesman Problem (TSP).

For the initial version, only Prim's algorithm is used.
Whilst this results in a Minimum Spanning Tree (MST) and not a TSP, the resulting images can still be pleasing.
This implementation of Prim's algorithm is also `O(n^2)` and will not scale well for large inputs.
For tuning, use the `simplify` command line option.

Finally, the solver allows for use of two different distance calculators: L1 and L2.
L1 distance is commonly known as [Manhattan distance](http://en.wikipedia.org/wiki/Taxicab_geometry)
and is the distance it'd take you to get from one point to another if you had to navigate via city blocks.
L2 distance can be described as the distance 'as the crow flies'.
Manhattan distance encourages horizontal and vertical lines which serve a particular aesthetic aim.

    Usage: aail [options] input_image output_image
    
    Options:
      -h, --help   show this help message and exit
      -n SIMPLIFY  Simplification amount (retain 1/n vertices for MST)
      --l1         Enable L1 (abs(x) + abs(y)) distance calculation instead of L2
                   (x**2 + y**2)

![](https://github.com/smerity/aail-art/raw/master/sample.png)
