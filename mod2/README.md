__Classification__

Given $N$ samples $\lbrace (\vec{x_1},y_1),(\vec{x_2},y_2), ⋯, (\vec{x_N},y_N) \rbrace$, 
- $\vec{x_i}$: feature vector of sample $i$
  - $\vec{x_i}∈X$, sample or features space
- $y_i$: sample $i$'s label or class
  - $y_i∈Y$, label or class space

Training a machine learning model $m_{\vec{α}}: \hat{y}=m_{\vec{α}}(\vec{x},y)$ is the process of optimizing its parameter vector $\vec{α}=(α_1,α_2,⋯,α_M)$ in its parameter space $\mathcal{Α}$ to find the $\vec{α^*}$ which maximizes a scoring function $s:X×Y→R$,

$\displaystyle s^*=argmax_{\vec{α^*} \in \mathcal{Α}} s(\hat{y},y)=argmax_{\vec{α^*} \in \mathcal{Α}} s(m(\vec{x},y),y)$

- $R$: real number

__Topics__
- [Classification model training and evaluation](./cmte.ipynb)
- [Support vector machines](./svm.ipynb)
- Decision trees
- Ensemble learning and random forests