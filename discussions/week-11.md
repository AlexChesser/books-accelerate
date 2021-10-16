# Week 11: Chapter 24 & 25 & 26 Partial Boudries, Layers and Boundries, The Main Component

## Chapter 24 Partial Boudries

- architectural bouraries are expensive
- they take a LOT of extra work NOW for a payoff LATER which may not ever happen as requirements change and we learn ne things about the system.
- in many cases the effort to separate can be deemed too high
- three options for dealing with this
  - skip the last step
    - in these cases, consider doing everything you can to make them easy to split, but leave them in the same component.
    - be warned that over time, without attention boudaries in these skip-the-last-step systems will weaken
  - one dimensional boudaries
    - outer rings can depend on inner rings, but don't worry about making two-way separations 
  - facades
    - have a class load all the other classes
    - be warned of the transitive dependency
    - consider a way to STUB other loaded classes when not needed
    
### Conclusion 

- part of the job is deciding what will probably need to be separated one day.
- important to consider this while designing a system

## Chapter 25 Layers and Boundries


## Chapter 26 The Main Component
