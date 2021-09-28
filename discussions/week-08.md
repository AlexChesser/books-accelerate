# Week 8

## Week' soverview

The core content of this week's chapters are a lot of repetition from previous ones. In an effort to avoid wasting time I'm going to leave out everything that isn't particularly new.

If I was designing a university course aroud this content I'd either group this chapter with previous ones, skip it or, organize the content around subjects.

## Ch 17 Boundreis: Drawing Lines

- recall the purpose of architecture is to minimize the human resources cost of changing the system.
- _Coupling_ is recognized as a cost in this chapter
- The author tells two stories of their experiences working on software systems
- the first is a cautionary tale about over-engineering
  - the specifics aren't terribly important, but could be summarized as someone drawing boundries too early
  - project failed under the weight of overwhelming complexity
- the second story was an example of deferring a decision through the use of interfaces. 
- Result was a system where they initially thought they needed a database, but eventually discovered they didn't need one

- the chapter's claim is that we need to draw lines between things that matter and things that don't
- the "things that matter" are defined as policies in a later chapter
  - for now, we accept that they're the business rules
- things that "don't matter" are said to be specific technologies (for example which brand of database you use)

- the chapter goes on to give additional concrete examples of "boundreis" we can draw with examples 
- the first is an argument around separating business rules from the database
- the second is an argument aroud separating business rules from the GUI (actually called it I/O)

- this system is said to be the way that third-party-plugins are enabled withing a project
- while changes of things like the GUI or the database are not necessarily simple, they're POSSIBLE

### Plugin Architectures

- exaple of a plugin system:  Visual Studio Code vs. the git plugin inside it
- thought question: which piece is "in charge" in the system? (VSCODE)
- the example is clearly that VSCODE could disable a plugin by changing their system but a plugin cannot disable VSCODE
- this is the level of isolation we want in our internal modules

### Conclusion
- this is effectively the single responsibility principle
- in order to be able to draw boundreis we need to partition our system into components

## Ch 18 Boudry Anatomy
