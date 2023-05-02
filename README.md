R Tree Implementation using CBS Algorithm
A R-tree is a spatial indexing data structure used to efficiently store and query spatial data in multi-dimensional space. It is commonly used in geographic information systems (GIS) and databases. The R-tree works by partitioning space into smaller regions called "nodes". Each node contains a set of objects, and each object is associated with a minimum bounding rectangle (MBR) that encloses it. Nodes can either be leaf nodes that contain actual objects or index nodes that contain references to other nodes. The structure of the tree is determined by a set of rules that govern how nodes are split and merged as objects are added or removed from the tree.

The CBS algorithm, which is used for splitting the nodes in the given R tree, works by recursively partitioning a scene's bounding box into two halves along one of its axes, and then repeating this process on each resulting half until a stopping condition is met. The algorithm selects the splitting plane by choosing a corner point of the bounding box and finding the axis along which the largest variation in object positions occurs. This axis is used as the splitting plane, and objects are partitioned into two halves based on their relative position to the splitting plane.

Installation
Download the file finalproject.c and run the script file in your VSCode terminal.

gcc -c finalproject.c
gcc -o exe finalproject.c
./exe
Usage
Input the data points into a data file named data.txt for inserting the same into the R tree data structure.

Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Reach out if you have any doubts or want to improve the code.

Please make sure to update tests as appropriate.
