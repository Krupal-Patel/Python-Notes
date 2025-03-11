# Softmax and ReLU: From Candy to Math

## Softmax: Sharing Candy, Then Probabilities
Imagine you’re sharing candy with friends: the kid who loves candy most gets the biggest pile, but it all has to add up to 100 pieces total. **Softmax** does this with numbers—it picks who’s “best” and makes everything fair!  

Now, mathematically, softmax transforms a vector $\mathbf{z} = [z_1, z_2, \dots, z_n] \in \mathbb{R}^n$ into a probability distribution:

$ \sigma(\mathbf{z})_i = \frac{e^{z_i}}{\sum_{j=1}^n e^{z_j}}, \quad i = 1, 2, \dots, n $

Each output $\sigma(\mathbf{z})_i \in (0, 1)$ and $\sum_{i=1}^n \sigma(\mathbf{z})_i = 1$. The exponential $e^{z_i}$ amplifies larger inputs, and the normalization ensures a valid distribution. Its gradient, crucial for optimization, is:
$$
\frac{\partial \sigma(\mathbf{z})_i}{\partial z_j} = \sigma(\mathbf{z})_i (\delta_{ij} - \sigma(\mathbf{z})_j)
$$
where $\delta_{ij}$ is the Kronecker delta (1 if $i = j$, 0 otherwise). Softmax is translation-invariant ($\mathbf{z} + c$ yields the same output), and in practice, we compute $\mathbf{z} - \max(\mathbf{z})$ to avoid numerical overflow. It’s perfect for classification outputs in neural networks.

**Example**: $\mathbf{z} = [1, 2, 3]$ → $\sigma(\mathbf{z}) \approx [0.090, 0.245, 0.665]$.

---

## ReLU: Light Switch, Then Thresholding
Think of a toy light switch: push it up, the light glows; don’t push, it’s off. **ReLU** is that switch for numbers—positive ones stay, negatives turn to zero!  

Formally, the Rectified Linear Unit (ReLU) is:
$$
f(x) = \max(0, x)
$$
Or piecewise: $f(x) = x$ if $x > 0$, else $0$. It’s defined on $\mathbb{R}$ with range $[0, \infty)$. ReLU is continuous but non-differentiable at $x = 0$, where the subgradient is typically 0 or 1. The derivative is:
$$
f'(x) = 
\begin{cases} 
1 & \text{if } x > 0, \\
0 & \text{if } x < 0 
\end{cases}
$$
This sparsity (zeroing negatives) and non-saturating nature make ReLU computationally efficient and mitigate vanishing gradients in deep networks. Variants like Leaky ReLU ($f(x) = \max(\alpha x, x), \alpha < 1$) address the “dead neuron” issue for negative inputs.

**Example**: $f(-2) = 0$, $f(0) = 0$, $f(3) = 3$.

---

Softmax handles multi-class probabilities, while ReLU drives nonlinearity in hidden layers—together, they power modern neural architectures!

> **Note**: Equations use LaTeX with `$...$` (inline) and `$$...$$` (display). On raw GitHub, they’ll appear as text unless rendered with MathJax (e.g., via GitHub Pages or extensions). For plain text, think of softmax as e^z_i / (sum of e^z_j) and ReLU as max(0, x).
