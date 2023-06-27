# Autograd-engine

A scalar-valued automatic differentiation engine that supports operations like addition, subtraction, multiplication, division, and exponentiation.

A directed acyclic graph internally keeps track of all the arithmetic operations and computes the gradients locally which are later used during backpropagation for minimizing the overall cost with respect to the weights and biases used.

Visualization of the graph could also be done by invoking the draw function on the final result variable. for eg: c = a+b, invoking draw(c) prints out the graph that is maintained internally.
