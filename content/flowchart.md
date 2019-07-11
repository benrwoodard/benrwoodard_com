---
title: "Flowchart"
date: '2019-05-06'
tags:
- opportunities
- communication tools
---

```{r, setup,echo=FALSE,warning=FALSE}
library(DiagrammeR)
library(fontawesome)

data(mtcars)
mermaid("
graph TB
        A(Ask to understand the<br> business question.)
        B(Summarise the business expected<br> results in a hypothesis.)
        C[Get the data and clean it.]
        D{Run the analysis}
        E(Communicate the Results)
        F(Communicate the what <br>to do with it.)
        A-- Start -->B; B--Something<br> Here Now ---C; C---D; D-->E; D-->F
")
```
```{r additional, setup,echo=FALSE,warning=FALSE}
fa("r-project", fill = "steelblue")
```