# Federated infrastructure

## Overview of Meeting

- What is Federated Infrastructure?

- How to share resources
- How is it managed and funded?

- Who are the users of federated infrastructure?
  - PIs, projects
  - Pipelines, operational groups

- Science driver example: using LSST data to follow up on different instruments
  - How can one get access to all the resources required?

- How can users describe their jobs?
- How to move work to the place with the right configuration, including data, processing resources, etc.
- How to discover the computing cababilities available in a federation.

- How to optimize a job?
  - data locality is not always the best solution.

- Standardization helps
  - data models for querying
  - VO protocols for data, authorization
  
- Can commercial computing be the answer most of the time?  What are the limits?

## Meeting details

- If you have access to resources, it would be nice to incorporate those resources into your processing/storage.

- How to run queries/processing on disparate collections?

- At what level to you integrate?
  - containers?
  - don’t expose the user’s to the notion that the resources are federated?
  - data models / CAOM for cross querying
  - for infrastructure: 
    - flexible data centre - some things shared, some not. 
    - isolation of work
 
- Nice to have the ability to send remote jobs and retrieve results at remote centres.

- Can science platforms be interoperable?

- If you have a data intensive job to run on a collection and have some money, you could by the infrastructure/computing or perhaps make a bid for the work to be done?

- Just use commodity computing when possible, but in some grants one is unable to buy services for computing, only hardware/software/people.

- How portable is a pipeline/job?  Move it to your laptop, another data centre?

- Containers can capture the work.

- Use cases:
  - Move work to the place with the right configuration, including data, processing resources, etc.
  
- How to decide where to send the jobs
- can we describe the way to capture the capabilities of a data centre

- Can the funded resources cooperate more efficiently?
- If you have a compute intestive job, you don’t care where it runs, only that it runs.
- Can users had work off to a broker to negotiate the work?

- Can cloud computing just solve this all?

- If you can describe you job well enough, rent out the resources.
  - needed to make the evaluation of the resources required

- What is the utilization rate of compute resources?
  - good, but could be better
  - elastic computing needed
  - NSF funded centres are still oversubscribed

- data locality is not always the best answer

- Problems
  1) how to find/schedule the compute resources
  2) certain data is required for the job
  
- If you have dependencies on, say a relational DB, how can you make it portable?

- What are the current supercomputing capabilities?
  - posix, local storage

- What are the common services that jobs need in a science platform.

- What is the value of federated computing?
  - funding silos can be in the way
  - can federated computing help solve this?

- Science drivers:
  - Using LSST data to follow up on different instruments
  - How can one get access to all the resources required?
  - Make it easy for scientists to get access to all that’s needed

- Operational drivers:
  - to help achieve operational requirements for efficiently

- Experiment with interoperable authorization through IVOA groups

- Summary question:  how to make it easy / realistic / happen for people to use infrastructure at different institutes in the same or similar way.  











 

