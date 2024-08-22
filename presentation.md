# Deep Feedforward Networks

- Synomymns includes: Multilayer Perceptrons (MLPs)

- Great for supervised learnings

- They are called feed foward because information flows throug the function being evaluated from **x** -> intermediate functions -> output **y** and there's no feedback.

- Called networks because they are typically represented by composing together many different functions.
  _`f(x) = h(g(p(x)))`_ with **x: input layer**, p(.) being the first layer, g(.) being the secon layer and h(.) being the third and **output** layer.

- The **Depth** of model is the length of the chain (Above, depth = 3)

- **Hidden layers** are those which do not have any direct contact or influence by the input layer (containing the trainig data)

## 1- Understanding Deep Feedforward Networks

- Linear models has limitation because not all problems are linear

- To extend linear models, to represent non-linear functions of x, we can apply the linear model not to x but the transformed input `φ(x)` a non linear transfo.

- We need to learn φ using our model `y = f(x; θ , w) = φ(x; θ)'w`

## 2- Example: Learning XOR
- You know what XOR does

# The XOR function

| A | B | A XOR B |
|---|---|---------|
| 0 | 0 |   0     |
| 0 | 1 |   1     |
| 1 | 0 |   1     |
| 1 | 1 |   0     |

- The XOR function provides the target function

- `y = f∗(x)` that we want to learn. Our model provides a function y = f(x;θ)

- Our learning algorithm will adapt the parameters θ to make f as similar as possible
to f∗(.) .

- Input vectors `X = {[0, 0]' , [0,1]',
[1, 0]', and [1, 1]'}`

- Linear models cannot learn the XOR function because the function is not a linear function at all.

