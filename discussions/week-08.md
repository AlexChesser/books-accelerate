# Week 8


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

## Ch 18 Boundry Anatomy

- Crossing boudry lines is as simple as one component calling a function in another
- The "cost" of this can be relatively inexpensive (calling into a DLL) or more expensive (calling a networked service)
- Boundries can also exist within a monolith 
- be compiled into a single package, they do not need to be visible to the end user

- threads are not considered "boundries"

### Local processes

- Local Processes _are_ considered boundrieds
- LP are defined (simply) as something like having your first EXECUTABLE running another EXECUTABLE
- important detail is that processes exist in separate memory space. they cannot access each other's memory except through interfaces
- communication could be through sockets or other OS level things like message queues, "mailboxes" (I don't know what mailboxes are)
- the goal of building this way is to protect lower-level components from higher level ones.
- (lower level is defined as more "important" or things that matter

### Services

- services are the "strongest" boundry level
- services are said to be slower than other options
- even when talking about "operating system services" versus network services

### Conclusion

- most systems (other than the monolith) use multiple boundry strategy
- "local boundries" are a good choice for "chatty" systems that need high communication
- services (local and network) are more ideally chosen for operations that are less worried about latency (or are designed with latency in mind) 
