# WEEK 06 - Component Coupling

A summary of this week's chapter is pretty simple make sure your code dependencies have no "cycles" which is to say all dependencies should flow in one direction only.

## the Acyclic Dependencies Principle

> allow no cycles in your component dependency graph

- the author introduces two concepts:
  - *morning after syndrome*: cod you were working on earier doesn't work in future because another developer changed a component elsewhere
  - *the weekly build*: in order to ensure MAS doesn't happen you reduce deployment frequency
  - both are listed as problems (with good reason)
  
### eliminating dependency cycles

- the solution is to partition the development environment into reusable components
- patitioned components must be appropriately versioned so OTHER components can decide when to update their dependency
- changes in partitioned components do not need to have an immediate effect on other teams
- to make this work you must monitor, manage and, maintain the dependency structure over time
- there can be no "cycles" or cirrcular dependencies

![Directed Acyclic Graph (DAG)](https://user-images.githubusercontent.com/355561/133002424-901c9ee9-98c3-439f-94d9-111c56fcac4b.png)

### The effect of a cycle in the DAG

![The effect of a cycle in the DAG](https://user-images.githubusercontent.com/355561/133002634-ec9ef62c-8e88-412f-8c47-32faa3365502.png)

- when there are cycles in your dependency graph it can be difficult to figure out what order to build your components in.

### Breaking the Cycle

- one option is to apply the dependency inversion principle

![inverting a dependency with an interface](https://user-images.githubusercontent.com/355561/133002927-c9921ea1-88a2-43d6-b971-89ca402d8442.png)

- another option is to create a new component which both components depend on.

![breaking the cycle with a new component](https://user-images.githubusercontent.com/355561/133003150-59faf94a-6798-4318-97e9-a968a55944dd.png)

### The Jitters

- This dependency flow issue is an ongoing process which requires it be constantly monitored over the lifetime of your project.
- component structure cannot be designed from the top down, insttead it is a system that evolves over time as the system  grows and changes
- component structure cannot be planned effectively in advance
- component flow diagras do nothing to describe the FUNCTIONALITY instead they describe the BUILDABILITY and MAINTAINABLILTY of a project

## the Stable Dependencies Principle

> depend in the direction of stability

- designs cannot be static.
- some components must be volotile
- we should plan for volatility by ensuring the more volatile a component is the less likely we are to depend on it
- many factors make a component hard to change
  - size
  - complexity
  - clarity of code
  - number of other components that depend on it

![the responsible component should be designed to be mroe stable](https://user-images.githubusercontent.com/355561/133003658-c04729fb-36ed-4034-b698-3b75e19638c8.png)

![the dependant component can be designed to be more volitile](https://user-images.githubusercontent.com/355561/133003706-a7dbcd7f-2537-4413-872e-c0b83ffb40b6.png)

- The component in the above diagram may contain only an interface as such it may be referred to as an ABSTRACT compnent.

### Stability metrics

- the author spends a lot of time discussing making stability _measurable_
- he presents multiple formulas based on number of dependencies and dependents
- in theory we should calculate stability and work to reduce that by adopting the techniques above (DIP and Shared dependencies).
- not worth digging into the complexity formulas, consider IDE tools may exist which do these calcualtions for us

## The Stable Abstractions Principle
 
