Prediciting cost
* Number of users
  - User workflows
  - spikiness of the traffic/usage
  - planning out secenarios
  - cost = users * user_niceness
* Segmentation and optimazation
  - Astrononmey says I need more resource
* What are the advantages (Steve at IPAC)
  - Cost + IT optimization
  - what do we need to track in order to prevent unexpected costs
  - kubernetes allows you to change the pod size dynamically
  - how has the shift from private to public cloud changed how we track costs
  - Considerations about doing a hybrid cloud
  - Steve: cpu/memory is realtively bounded, storage and bandwitdth are harder to predict
  - Adding data to the datacenter or cloud is a fixed cost
    - Retrival costs are not fixed and can be unpredictable in the could
  - How do you manage idle/abandoned resources?
    - jupyterhub is working on  downsizing the cluster automatically based on idle sessions
    - containers are ephermeral, storage is not
    - idea of hot vs cold storage
  - What about unintentional long term usage (long term jobs / bitcoin mining)
    - Christian thinks logging/metrkcs is probably the answer
    - K8s dashboard can help determine system abusers
    - Possibly provide a new admin tool for jupyterhub
    - Kubernets dashboard demo from Mathias NCSA
      - Demo for watching containers start and stop
      - This transitioned into the Mathias's kubernets demo
