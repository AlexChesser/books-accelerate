# WEEK 06 - Component Coupling

A summary of this week's chapter is pretty simple make sure your code dependencies have no "cycles" which is to say all dependencies should flow in one direction only.

## the Acyclic Dependencies Principle

> allow no cycles in your component dependency graph

- the author introduces two concepts:
  - *morning after syndrome*: cod you were working on earier doesn't work in future because another developer changed a component elsewhere
  - *the weekly build*: in order to ensure MAS doesn't happen you reduce deployment frequency
  - both are listed as problems (with good reason)
  
## eliminating dependency cycles

- the solution is to partition the development environment into reusable components
- patitioned components must be appropriately versioned so OTHER components can decide when to update their dependency
- changes in partitioned components do not need to have an immediate effect on other teams
- to make this work you must monitor, manage and, maintain the dependency structure over time
- there can be no "cycles" or cirrcular dependencies

![Directed Acyclic Graph (DAG)](https://user-images.githubusercontent.com/355561/133002424-901c9ee9-98c3-439f-94d9-111c56fcac4b.png)

## The effect of a cycle in the DAG

![The effect of a cycle in the DAG](https://user-images.githubusercontent.com/355561/133002634-ec9ef62c-8e88-412f-8c47-32faa3365502.png)

- when there are cycles in your dependency graph it can be difficult to figure out what order to build your components in.

## Breaking the Cycle

- one option is to apply the dependency inversion principle

![inverting a dependency with an interface](https://user-images.githubusercontent.com/355561/133002927-c9921ea1-88a2-43d6-b971-89ca402d8442.png)

