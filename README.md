# Scalar Grad

Inspired by Andrej Karpathy's [micrograd] (#https://www.youtube.com/watch?v=VMj-3S1tku0)

Scalar grad is a scalar-valued automatic differentiation engine that supports operations like addition, subtraction, multiplication, division, and exponentiation.

A computational graph internally keeps track of all the arithmetic operations performed and computes the gradients locally which are later used during backpropagation for minimizing the overall loss. This library can be used for developing a simple neural network like a binary classifier.

Visualization of the graph could also be done by invoking the draw function on the final result variable. 
for eg: 

```
c = a+b
draw(c)
```

invoking draw(c) prints out the graph (similar to the one in the notebook) that is maintained internally.
