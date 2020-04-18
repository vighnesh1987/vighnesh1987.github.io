---
title: Master the System Design Interview in 5 nanoseconds!
date: "2017-05-08"
---

I was helping out a friend preparing for system design interview questions. That prompted me to do a brain dump of the patterns I had observed during my last interview season in late 2016. Figured it might be useful for others too.

## Common patterns

1. Understanding of load balancers including various routing paradigms — sticky/non-sticky/round-robin

1. Sharding and picking a good shard key so that you can run the most dominant query on a single shard

1. Design RESTful (or not) APIs

1. Figure out how to push messages to clients (websockets, etc)

1. Fan-in/Fan-out problem

1. Understanding of messaging queues (Kafka etc) and how they can be used within your backend system

1. Database choice — SQL vs NoSQL (should be able to provide some reasoning for your choice)

1. Data modeling the problem for the database of your choice

1. SQL primary keys, foreign keys, [what indexes you will use](http://use-the-index-luke.com/) and ability to write JOINs

Keep googling using keywords listed in each of these bullet points and read/watch till you understand these terms. Rest of it is really a matter of doing enough system design interviews, screwing them up and learning from where you went wrong.

## A couple of good resources

1. https://github.com/donnemartin/system-design-primer
2. https://www.hiredintech.com/classrooms/system-design/lesson/52

## Approach

As is the case with any interview, the first step involves asking a lot of questions. I found it harder to come up with good questions in system design interviews as compared to coding interviews. A couple of approaches helped here.

A friend of mine told me to think of the system as a black box with inputs and outputs. Then a good way to figure out what questions to ask is to try and hammer down all the various inputs and outputs for the system

Another approach that might work well is to mock out the front-end for which you are trying to build a backend system. And then trace the actions that you can take on the mock and verify with the interviewer if those actions are within the scope of what you are trying to achieve. Focus on minimizing the scope as much as possible. This is important to keep in mind because system design questions tend to be phrased very loosely.

## Closing thoughts

If you find yourself struggling at these questions, it indicates that you probably haven’t worked on large scale complex systems and it may serve you well to factor that in when you pick your next job.
