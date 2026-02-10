# Notes — Hyperparameter Agent for Probabilistic Solvers
*A minimal, physics-informed architecture*

---
## Structure of the notes 
1. Motivation and Personal Framing 
2. The big picture: understanding the problem
3. What Goes In / What Comes Out
4. From Problem Structure to Experimental Controls
5. Representation: What Does the Agent Actually See?
6. Predict, Refine, Remember 
7. Learning Strategy 

## 1. Motivation and Personal Framing

Before focusing on a specific technical solution, I like to start by understanding the system as a whole: what already exists, what is expensive, where feedback comes from, and where uncertainty actually lives.

This perspective comes from my background in physics. I find it difficult to design components in isolation without first building a mental model of the full pipeline. For me, architecture emerges from understanding interactions, constraints, and failure modes not from assembling modules independently.

In this problem, I am not trying to propose a universal or optimal solution. Instead, I treat this as a minimal “hello-world” architecture: a concrete, simple example of how one might approach hyperparameter selection for probabilistic hardware solvers.

My goal is to explore how problem structure, physical intuition, and limited feedback can be combined into a system that proposes reasonable operating regimes, under realistic constraints such as expensive hardware access, imperfect simulators, and noisy outcomes.

I see hyperparameter selection here not as a standard machine learning task, but as a form of experimental control. Small changes in parameters can qualitatively alter solver behavior, meaning we are effectively designing how a physical system explores an energy landscape.

Because of this, I approach this problem as a systems and physics-informed design challenge.





