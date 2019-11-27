# System Design Interview Framework :memo:

This document defines a suggested system design interview structure, which can be used as a guideline. Please feel free to open a PR with suggestions!

## Interview Steps

### 1. Identify functional requirements
* TODO

### 2. Identify non-functional requirements

* How can we tell that the system is working?
* Is there a bottleneck in the design?
* How do the components work together?
* How do we provide great service to everyone?

### 3. Identify main stakeholders of the system

### 4. Define expected APIs

### 5. Back-of-the-envelope calculation

* What scale is expected from the system?
* How much storage will we need?
* What network bandwidth usage are we expecting?

#### Numeric estimates for properties like this:

* Latency
* Throughput
* Storage

#### Cost of operations:

* Read from memory
* Read from disk
* Local area network (LAN) round-trip
* Cross-continental network


### 6. Define data model


### 7. Create high-level design (draw a block diagram)

### 8. Create detailed design (cache, replicas, detalization of individual components)

* Since we will be storing a massive amount of data, how should we partition our data to distribute it to multiple databases? Should we try to store all the data of a user on the same database? What issue could it cause?
* How will we handle X?
* What data access models will we have?
* How much and at which layer should we introduce cache to speed things up?
* What components need better load balancing?

### 9. Identifying bottlenecks

* Is there any single point of failure in our system? What are we doing to mitigate it?
* Do we have enough replicas of the data so that if we lose a few servers we can still serve our users?
* Similarly, do we have enough copies of different services running such that a few failures will not cause total system shutdown?
* How are we monitoring the performance of our service? Do we get alerts whenever critical components fail or their performance degrades?
* How does system respond to various failures

### 10. Add telemetry: monitoring, logging


## Must know

* Sharding data
* Replication types
* Write-ahead logging
* Separating data and metadata storage
* Load distribution

## General guidelines

* Layout trade-offs and compromises and explain reasoning.
* Explain thought process
* Keep going, don't stop, don't give up.

## Resources

* TODO 
