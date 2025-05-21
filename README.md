# User-Equilibrium-UE-System-Optimal-SO
This script computes the static traffic assignment using the Frank-Wolfe algorithm (FW) or the Method of successive averages (MSA).

It can compute the User Equilibrium (UE) assignment or the System Optimal (SO) assignment.

The travel time cost function that models the effect of congestion on travel time is pluggable and definable by users.

The cost function available are:

- BPR cost function ([see more](https://rdrr.io/rforge/travelr/man/bpr.function.html)).
- Greenshields cost function (see Greenshields, B. D., et al. "A study of traffic capacity." Highway research board proceedings. Vol. 1935. National Research Council (USA), Highway Research Board, 1935.).
- Constant cost function (no congestion effects).

Our implementation has been tested against all the networks for which a solution is available on [TransportationNetworks](https://github.com/bstabler/TransportationNetworks) and has always obtained the correct solution.

# How to use
First, clone the repository to a local directory.

To use the algorithm, simply call the `computeAssingment()` method in the `assignment.py` script. If you prefer Jupyter Notebook, simply use `ComputeAssingment.ipynb`.

The documentation of the method in `assignment.py` provides a through description of all the available parameters and their meaning.

# Importing networks
 Networks and demand files must be specified in the TNTP data format.
 
 A through description of the TNTP format and a wide range of real transportation networks to test the algorithm on is avaialble at [TransportationNetworks](https://github.com/bstabler/TransportationNetworks).

 
