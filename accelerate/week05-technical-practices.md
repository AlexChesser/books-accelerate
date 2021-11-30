# Technical Practices

`[![Week Five Video](https://img.youtube.com/vi/*******/0.jpg)](https://www.youtube.com/watch?v=*******)`

## it starts with extreme programming (XP)

- XP prescribes
  - test driven development
  - continuous integration
  - continuous delivery 
- the rationale is that they enable more frequent, higher quality, safer code releases
- continuous delivery has a measurable impact on business outcomes

## Continuous Delivery (CD)

### five keys to CD

- **Build quality in**: cease dependence on inspection to provide quality (automate testing)
- **work in small batches**: smaller chunks of work which deliver measurable business value quickly
  - obtain feedback early
  - allows you to avoid work that delivers zero or negative value to the company
  - change the economics of the build process such that the cost of new changes is very low
- **computers solve repetitive tasks, people solve problems**: invest in automating toil
  - (again, automate testing)
- **relentlessly pursure continuous improvement**  
- **everyone is responsible**: focus on organizational goals over departmental goals

### foudations of CD 

- **Comprehensive Configuration Management**: provision environments from code / version control
- **Continuous Integration**: keep branches short lived (less than a day's work)
  - integrate frequently into trunk/main branch
- **Continuous Testing**: developers should be able to run all tests on their own machine 
  - they shold run frequently and be fast
  - developers will be able to locally triage and fix defects

### On Version Control (VC)

- all application code should be in VC
- all system configuration shold be in VC
- application configuration
- scripts automating build and config

- when taken together there is a significant impact on performance
- decreased deployment time
- decreased team burnout
- teams that do well with CD identify more strongly with the organization they work for (retention?)
- improving CD appears to improve organizational culture

- two things that are highly coorelated with CD
  - loosely coupled, well encapsulated architecture
  - teams which self select their tools

### Impacts of continuous delevery 

- brings a payoff in the way the work _FEELS_
- investments in technology are investments in _PEOPLE_ resulting in
  - lower levels of deployment pain
  - reduced team burnout

![Structures influencing Continuous Delivery](https://user-images.githubusercontent.com/355561/143177891-f2d66b24-537c-494a-a55f-790b22cd11da.png)

![Effects of continuous delivery](https://user-images.githubusercontent.com/355561/143178179-578c86a0-3424-41df-8b6d-2d85f51b9fd1.png)

- continuous delivery systems impact software quality 
- result in less rework 
- result in less unplanned work
- both of the above are useful proxies for quality 
- consider "unplanned work" as equivalent to paying attention to the low-fuel guage vs. running out of gas on the highway

### CD practices that work

- **version control**: hopefully obvious
  - keeping system and application configuration in version control is highly correlated with performance
- **test automation**: reliable automated tests help delivery 
  - fragile tests should be in quarrantine
  - code becomes more testable when developers write the tests
  - when developers are responsible for tests they care more about them
- **test data management**: having a robust and reliable set of test data to work with is **known** to be hard, but also valuable
- **trunk based development**: merging code back into main frequently is correlated with performance
  - long lived branches get stale
  - compare to the process of [git-flow](https://docs.github.com/en/get-started/quickstart/github-flow)
-  **information security**: more likely to include security earlier in their process
  -  integrating security practices early is strongly correlated

## Adopting Continuous Delivery

- CD improves delivery performance & quality
- improves culture
- reduces burnout
- reduces deployment pain
- implementing CD often requires rethinking everything
- requires relentless work to
  - simplify architecture on an ongoing basis
  - ensure automation isn't prohibitively expensive

- a critical obstacle to implementing CI/CD is application architecture 

dun dun dun ... which we talk about in the next chapter  :D  
