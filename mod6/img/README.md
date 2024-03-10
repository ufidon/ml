fig1: an MLP that can solve the XOR classification problem
---
```mermaid
flowchart LR
  x1["x1"]
  x2["x2"]
  y["y"]
  a1(("p1<br>b1=-3/2"))
  a2(("p2<br>b2=-1/2"))
  a3(("p3<br>b3=-1/2"))
  x1-->|"1"|a1
  x1-->|"1"|a2
  x2-->|"1"|a1
  x2-->|"1"|a2  
  a1-->|"-1"|a3
  a2-->|"1"|a3
  a3-->y
```

fig2: A typical MLP
---
```mermaid
flowchart BT
  x1["x1"]
  x2["x2"]
  y1((" "))
  y2((" "))
  h1(("Σ⎇"))
  h2(("Σ⎇"))
  h3(("Σ⎇"))
  o1(("Σ⎇"))
  o2(("Σ⎇"))
  x1-->h1
  x1-->h2
  x1-->h3
  x2-->h1
  x2-->h2
  x2-->h3
  h1-->o1
  h1-->o2
  h2-->o1
  h2-->o2
  h3-->o1
  h3-->o2
  o1-->y1
  o2-->y2
```

fig3: wide & deep nn
---
```mermaid
flowchart LR
  i("Input layer")
  n("Normalization")
  h1("Hidden1")
  h2("Hidden2")
  c("Concat")
  o("Output layer")
  i-->n-->h1-->h2-->c-->o
  n-->c
```

fig4: wide & deep nn with multiple inputs
---
```mermaid
flowchart LR
  iw("Input wide")
  id("Input deep")
  nw("Normalization")
  nd("Normalization")
  h1("Hidden1")
  h2("Hidden2")
  c("Concat")
  o("Output layer")
  id-->nd-->h1-->h2-->c-->o
  iw-->nw-->c
```

fig5: wide & deep nn with multiple inputs & multiple outputs
---
```mermaid
flowchart LR
  iw("Input wide")
  id("Input deep")
  nw("Normalization")
  nd("Normalization")
  h1("Hidden1")
  h2("Hidden2")
  c("Concat")
  o("Main output")
  ao("Auxiliary output")
  id-->nd-->h1-->h2-->c-->o
  iw-->nw-->c
  h2-->ao
```

