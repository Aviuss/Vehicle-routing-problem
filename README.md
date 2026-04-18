# Vehicle-routing-problem

task source: https://ktiml.mff.cuni.cz/~pilat/en/nature-inspired-algorithms/vehicle-routing-problem/

Your task will be to solve the so-called Vehicle Routing Problem (VRP) using the Ant Colony Optimization algorithm. VRP is essentially a generalization of the traveling salesman problem, where the goal is to optimize the delivery of shipments for a postal company. We are given depots, each with their own respective vehicles with a given capacity, which start and necessarily end their journey at the depot, and a set of shipments that must be delivered to their recipients. The task is to find a set of delivery routes such that all shipments are delivered to their recipients, and the total cost of these routes is minimized - that is, as few distribution vehicles are used as possible, and the routes are as short as possible.

In the context of this task, we will consider a simplified version of this problem, where we have only one central depot and an unlimited number of identical vehicles. You will optimize three instances of this problem, which you will receive as files in XML format - two small instances and one larger instance. Each input file contains the following:

    A list of nodes with their respective x and y coordinates determining their position in the world. A node of type 0 is the depot, and the other nodes of type 1 are customer locations.
    A list of vehicles (in our case, only one type of vehicle), along with their home depot and capacity.
    A list of customer demands (shipments), that must be delivered to their destination.

# Installation

```
python -m venv venv
source venv/bin/activate

pip install jupyter ipykernel numpy matplotlib
python -m ipykernel install --user --name=venv
```