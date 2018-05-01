Benefits of building an open source community around a platform

Joseph
Astroquery is a good example of a healthy community / workflow
Integrating science platforms with the different open source communities

Christian:
- Zero to JH example
  - Easier to learn
  - many new users try to help with docs off the bat

Erik:
Building a community around a platform
Building a community in a platform


Benefits of using open source projects close to the data

Integration with bug-trackers/issues
Can get people in the door

Sebastian:
How do we provide a unified interface to all of the distinct APIs / Datasets

Does VO* fill the void for that tooling?

Is it too much overhead/complexity?


Example: cross correlating panstars vs gaia, etc...
  How do we accomplish this

Erik:
* The bigger the data/project, the harder it is to get people hacking on it
* astropy as an example, afraid to break it
* Is a consolidated central interface too imposing to work on?


Christian
Can we distribute tools via containers which run on each other’s datacenters
Latency?

Sebastian:
Does not think so

Erik:
Butler is smart enough to blur the line between local resource and remote resources

Frossie:
Where does the logic go?
Containers are for software distribution.
JH containers are souped up versions of the above.

Erik:
Could be interpreted as vendor lock in

Frossie:
* Not trivial to make universal containers


Joseph:
* Can the locality be made transparent (EG dns)

Christian:
* PR astroquery
* be explicit on if we are using the “fast lane”

Erik:
* could auto detect your environment: try to tell the user you are using a 

Christian:
How do we distribute/force updates too toolchains or APIs

 

Joseph:
Treating the containers like software (eg pip)


Christian:
How collaborate

Robert:
Individual platforms or one platform to rule them all

Joseph:
Went to talks where whole project was on github.  What do maintainers experience, PRs, doc fixes, other benifits

Frossie:
Other people have deployed the LSST platform
Got some slack questions
Traditional science platforms tend to take a while to deploy (weeks?)
Working toward quicker releases
The easier it is to deploy your stack the easier it is for the community to get involved.

Christian:
What benefits do I get running the LSST stack at STSCI over just running your containers in my own platform?

Joseph:
And vicea versa


Frossie:
Better of using our containers in your platform.
Should be fairly seamless, less arguments expected.
Get auto updates if using a tagged release
You can scale it however you want


Sabastian:
Containers assume certain environment and other underlying services

Frossie:
Several different types of containers released
Christian’s question was the basic software, not the whole platform
Could use that container with docker directly if they wished
To get performance, qserve needs to run on bare metal
Data access services (API) is a k8s deployment


Christian:
If we were to deploy LSST Containers here, would we have access to your API which is part of the LSST hosted stack?  Would we need to run that ourselves?

Frossie:
Believes if deploying inside their own datacenter: it can do optimized access
Can deploy outside the datacenter: All the data access happens through the public APIs


Christian:
As we build our containers, we try to make it generic enough to run anywhere

Frossie:
Would require effort to adapt their container
Butler is smart enough to detect data center locality

Christoph:
Home directory mounts?  How can that be done dynamically
S3 access for HST?

Christian:
S3 support is opt in

Frossie:
We could deploy on a common cloud
We talk about commodity cloud, we don’t have a science cloud

Christian:
2 container layers
Default software container
JH container built on top

Christoph:
The whole idea is bringing the code to the data
Containers don’t solve this issue



Frossie:
Many places are duplicating the data sets in europe
Still an improvement

Christoph:
Ideally run the container in the environment nearest the data

Frossie:
Built in a platform independent way as a necessity
Code and data together is ideal

Christian:
I could be dominated by compute and would be easier to pay for my own compute and use your API for data access

Frossie:
Bandwidth is still limited
This is where science platform portability is critical: if you have regional data copies (eg. in Europe) as a European scientist you want to bring your code to THAT data copy, and therefore you want that data center to host a copy of the data AND a deployment of the relevant science platform. 

Why don’t we use astropy:
Performance
Harder to fund astropy work
Burned by other community projects in the past

