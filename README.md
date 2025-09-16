# Softmax A*

A simple implementation of A* with "softmax".

I've written this demonstration into a Jupyter Notebook.

## Algorithm

It's nearly A*, but with on difference.

Normally, in A*, at the start of a pass, we sort the "open set" according to the F-scores, and take the minimum score.

Here, we "flip" them (`V(i) = max(scores) / V(i)`), take the soft-max, divide by temperature, then sample.

## Demo

We run this for some number of executions, then form a heat map of edge traversals and render this with `networkx` and `matplotlib`.

