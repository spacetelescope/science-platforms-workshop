# Software Delivery

Issues brought during the session

## Delivering medium to compute nodes
* containers (docker, singularity, shifter), VMs
* HPC like file systems (lustre, GPFS...)
* CVMFS http file system delivery for very large software stacks
* singularity for arbitray user workflow
* pre-built container curated catalogue
 
## How to push software
* container registries
* locally managed docker repos
* longevity of code on commercial repos?

## Orchestrating software delivery
* **kubernetes**, swarm, mesosphere
    * is k8s complexity needed for simple server?
    * k8s networking abstraction
    * stateful services abstraction
    * federation between clouds
    * isolation from dev/prod environments
    * phased rollout version deployments
    * k8s for batch processing with other queue scheduler (celery)
    * stateful processes - maybe checkpointing on docker (experimental)
    * live migration still an issue
    * very developer friendly (CI/CD workflows)
* workflow 
* batch scheduling with HTCondor, SLURM?
* HA in the cloud
* Exposing batch jobs to the user (hiding orcherstration complexity)
* Create workflow of jobs as external service

## Interoperability

Containers vs. VMs?

