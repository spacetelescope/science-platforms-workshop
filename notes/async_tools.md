# Async tools

## Use cases & features

- What are the features you need to support?
  - Batch processing
  - Big queries
  - Submission of custom processing code (server-side analytics)
    - What sort of constraints can be put on this?
    - Cannot be done anonymously
  - Some kind of history mechanism (way to run old jobs)
    - Canceling, resubmitting (UWS has much of this)
  
- Where do you stage the result?
  - How do you clean up after users (when they're done using the space/resources)
- CASJobs has an 8-hour job limit. 
  - Sometimes need to execute a sequence of queries to fit in that window
  - Option to allow admin to run the query for them
- TAPS has both sync and async mode (based on USW - Universal Workflow Service)
- UWS is an IVOA standard
- NED decides whether to make a query async or not (based on pre-defined thresholds)
- Poll vs push to notebooks to receive updates (e.g. web sockets etc)
- Does async require user-registration?
  - If it's anonymous then necessarily be resource-limited
- Should users request resources (or be user-configurable)
- How to stop people from using crazy amount of resources.
- LSST want to enable users to be able to take their processing workloads and run on more traditional HPC resources (e.g. using Singularity)
- Large uploads and downloads
  - Globus as a potential solution
  - Parallelize downloads over HTTP
  - Wget/curl will restart downloads
  - GridFTP

## Technologies

- How can K8S help with processing?
  - e.g. Jobs that spawn containers?
- AWS Lambda
