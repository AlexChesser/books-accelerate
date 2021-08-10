# Week 01  - Introduction

## Chapters Read

Contents, Forward, Preface, Introduction, CH01, CH02 

### Contents

The TOC indicates that there are six broad sections to the book.

* *Introduction*: Martin defines software architecture and lays the case for his work.
* *Programming Paradigms*: Describes the different ways of programming (structured, functional, object oriented)
* *Design Principles*: The SOLID acronym is pretty famous, this section details each letter in detail. 
* *Component Principles*:  Looks like there's a step between principles and architecture... in the metaphor, perhaps these are bricks?
* *Architecture*: the reason we're here!
* *Details*: Interestingly, Uncle Bob separates a lot of stuff out from being classed as "architecture"  chapter titles like "the database is a detail" or "the web is a detail" seems to indicate that they're in some ways irrelevant to the discussion of software design principles. Looking forward to reading his arguments here :)   

### Forward

- "Architecture" is a metaphor describing the structure of the code
- Software is made out of software, it is fractal and recursive in its nature
- Architecture represents the *SIGNIFICANT* decisions in software design where significant is a meaure of the cost of changing it
- If you think good architecture is expensive, try bad architecture
- How do we reduce future development costs without knowing what is going to happen?

### Preface

- The author wrote his first line of code in 1964, this stuff is based on 50 years experience
- The rules of archtecture are the same across projects

### Introduction

- When software design is done right, it takes a fraction of the human resoruces to design and maintain

### Chapter 01 - What is Design and Architecture?

- There is no different between system design and system architecture. They refer to the same thing.
- The goal of architecture is to minimize the hhuman resources required to build and maintain the required system.
- **Case study**: 
  - As staff increases the product development speed slows and plateaus
  - As is slows and plateaus the cost (per productivity) increases exponentially (eg: [Phong Thieu tiktok](https://www.tiktok.com/@pgt__/video/6993791082811215110) )
- When little or no thought is given to the cleanliness of the code or the structure of the design, then development speed slows to a stop because of the complexity
- Well designed code matters
- "We can clean it up later" <-- but you never actually do. Don't feel back, nobody ever actually does. Take the lesson though and do it cleanly the first time.
- Making messes is always slower than staying clean from the start.
- **"Throw it out and start over"** is also effectively BS because if you don't run aggressively "clean" you will just rebuild with a new mess
- "Their overconidence will drive the redesign into the same mess as the original project"
- The best option for software development is to take the qulaity seriously from the start (later chapters define quality)
- on a long term the rules of architecture allow us to minmize effort and maximize productivity (eg: INTERFACES... )

### Chapter 02 - A Tale of Two Values
