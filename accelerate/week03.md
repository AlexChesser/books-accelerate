# Week 03 - Measuring Performance

- in order to move forward with measurement we need to come to an understanding of **what "good" means**
- it is expected that the software we build changes and evolves based on what we learn while building it.

## flaws in previous measurment techniques

- most measurements focus on productivity which suffers from the drawbacks

1. focuses on _outputs_ rather than _outcomes_
2. focuses on _individual_ / _local_ measures rather than _global_ ones

### bad examples
- lines of code (no need to discuss, this was an archaic measure)
- agile software measuring **VELOCITY** 
  - velocity has several flaws
  - relative and team dependant based on estimates
  - subject to being gamed estimates get inflated,
- utilization as a proxy for productivity
  - suffers from a lack of ability to pick up adhoc or unplanned work

## Measuring Software Delivery Performance

- a successful measure of performance should 
  - focus on global outcome
  - ensure teams aren't pitted against each other
  - focus on outcomes not output
  - shodln't reward busywork & toil

- _good_ metrics of delivery performance
  - delivery lead time
  - deployment frequency
  - time to restore service
  - change fail rate
  
- shorter delivery lead times are better since they allow for faster feedback
- DLT is the time it takes from code COMMITTED to main until that same code is running in production

- **batch size** is a term used in the manufacture of physical goods which represents high performance in manufacturing 
- a proxy for batch size in software prodcuction is deployment frequency

- delivery lead time and deployment frequency when taken together represent TEMPO

- the next criticial factors are around the inevitable failure
  - how quickly can service be restored after failure?
  - how frequent is failure? (what percentage fails?)


| 2017 |High Performers|Medium Performers|Low Performers|
|---   |---            |---              |---           |  
|Deployment Frequency|On demand (multiple deploys per day)|Between once per week and once per month|Between once per week and once per month*|   
|Lead Time for Changes|Less than one hour|Between one week and one month|Between one week and one month*|  
|MTTR|Less than one hour|Less than one day|Between one day and one week|  
|Change Failure Rate|0-15%|0-15%|31-45%|   
   
^* Low performers were lower on average (at a statistically significant level) but had the same median as the medium performers.

### findings

- there is no trade off between speed and failure.
- in fact higher performers deploy faster, more often, fail less, AND recover faster
- it appears robust and solid systems are REQUIRED to go fast
- the highest performers are moving further ahead of their competition

## Impact of delivery performance on organizational performance

- there is a predictive relationship between engineering performance and organizational performance
- organizations with high performing IT teams 
  - more profitable
  - greater market share
  - higher productivity 
- High performing orgs are **TWICE AS LIKELY** to exceed their goals aroud ROI as low performers
- High performing orgs also twice as likely to exceed their objectives om
  - quantity of goods and services 
  - operating efficiency
  - customer satisfaction
  - quality
  - achieving organizationsal "mission" goals

![This research has foud a precictive model](https://user-images.githubusercontent.com/355561/142114186-b59c92a5-9ecc-431f-b958-25496b673f8f.png)

### extrapolation 

- this evidence serves to present a STRONG argument against outsourcing of any software that is strategic to your business
- this however does mean that one should consider NOT building software taht is not core/strategic to the business
  - eg: payroll / ticket management / etc...
- distinguishing between strategic and non-strategic software is enormously important
- consider the [wardly mapping method](https://en.wikipedia.org/wiki/Wardley_map) 
  - <https://www.infoq.com/presentations/interview-wardley-maps/>
  - <https://www.youtube.com/watch?v=rnZdLv8InbU>

## Driving Change 

- the findings in ACCELERATE are beginning to move beyond correlation and into the realm of prediction
- **use these tools carefully**
  - if you work within a learning culture, you're probably fine, this stuff is super powerful
  - if you are in a "pathological" or bureaucratic org measurement is used as a tool of control
  - whenever there is fear in your system, you will get the wrong numbers

- to use these tools you must first understand and develop your company culture.

