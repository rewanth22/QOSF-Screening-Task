# QOSF-Screening-Task

Task 2 of the QOSF Screening task was implemented in python using PennyLane.

**Objective:** To implement a circuit that returns |01> and |10> with equal probabilities.

A parametric circuit is implemented with Gradient Descent to optimise the parameters to produce the required objective.

**Cost Function:** (P(|01>) - P(|10>))^2 + P(|00>)^2 + P(|11>)^2

- We need the states |01> and |10> with equal probabilities and we achieve that by subtracting their probabilities and squaring them so that when we get equal probabilities, that corresponding term equates to 0 and gives us a low cost.
- Also the cost function is designed in such a way that getting the state |00> or |11> increases the cost. This is done so that we do not get the states |00> or |11> by including their probabilities and squaring it.

