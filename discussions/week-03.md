# Week 3 - Design Principles  S.O.L.I.D

### A WARNING

- The chapters on SOLID principles do not dwell on explaining what SOLID principles ARE. If you have not yet learned them or want a refresher, take a moment to go through some content on them before proceeding (or cross your fingers :) that's OK too)
- The chapters ahead will focus on the SOLID principles implications for architecture
- some "refresher content"
  - a "children's book" on SOLID : https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898 
  - Wikipedia https://en.wikipedia.org/wiki/SOLID
  - <https://www.youtube.com/watch?v=zHiWqnTWsn4> from the author himself (80 minutes)
  - my personal favorite explanations are from Jason Weimann @ Unity3d.college they're very specific to writing games in Unity, but they're designed in a way which really makes the content "concrete" in a real way with a fun visual example. Plus, he has good production value. Don't forget if you watch on 2x speed you can get through it a lot quicker.
    -  S: <https://www.youtube.com/watch?v=Eyr7_l5NMds> (11 min)
    -  O: <https://www.youtube.com/watch?v=wYkzeKghjsI> (8 min) 
    -  L: <https://www.youtube.com/watch?v=eXPBR3WlRGY> (8 min)
    -  I: <https://www.youtube.com/watch?v=ll6bxQGkyCk> (10 min)
    -  D: <https://www.youtube.com/watch?v=fGshe3ILKnA> (15 min)

## Section III - Design Principles  

- The goal of SOLID principles are the creation of "mid-level" software structures that:
  - tolerate change
  - are easy to understand
  - are the basis of components that make can be used in many software systems (reusable?)
- mid-level code is defined as sitting at the "module" level. Which is to say more than a function, (potentially) less than a complete system.

- SRP: the single responsiblity principle - each software module has one and only one reason to change.
- OCP: the open-closed principle - code should be able to be changed by ADDING new code as opposed to changing existing code
- LSP: the Liskov substitution principle (attributed to Barbara **Liskov**) - parts must adhere to a CONTRACT that allows those parts to be SUBSTITUTED for one another.
- ISP: the interface segregation principle - avoid depending on anything that doesn't get used.
- DIP: the dependency inversion principle - code should not depend on DETAILS.

- In case you missed the warning above :) 
> the chapters in CL focus on the architectural implications of SOLID and not what SOLID *is*

**Further note**: these chapters get pretty dense from a technical perspective. It's a good choice to go slow instead of doing all 5 in one week :)

## Chapter 07 - SRP - Single Responsiblity
