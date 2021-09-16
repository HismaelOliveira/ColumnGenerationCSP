# Column Generation Algorithm to Cutting Stock Problem

In the column generation method only a subset of the variables is used initially. The method sequentially addes columns, using information given by the dual variables for finding the approriate variable to add.

The problem being solved is split into two problems: the **master problem** and the **sub-problem**. 

The **master problem** is the original column-wise formulation of the problem with only a subset of variables being considered. 

The **sub-problem** is a new problem created to identify a new promising variable. 

The *objective function* of the sub-problem is the *reduced cost of the new variable* with respect to the current dual variables, and the constraints require that the variable obeys the naturally occurring constraints.
