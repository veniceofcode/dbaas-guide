***Introduction***

Database is one of the key building blocks for a variety of applications. Currently most openshift customers run their databases on the same cluster, manage it themselves and provide access to developers. Database as a service makes this much simpler, allowing databases to run at a central location managed by database administrators allowing business to focus on their applications.

The Red Hat Database as a service add-on enables:

- Easy consumption of Database as a service from ISVs like MongoDB Atlas, Crunchy Bridge, and CockroachCloud on kubernetes clusters
- Easy management, monitoring and control by administrators of DBaaS consumption, usage, status across cluster and clouds
- Enables end to end managed support experience
- For Alpha release DBaaS Add-on enables ease of consumption for developers and simple management for administrators on one managed OpenShift Platform (OSD and ROSA) . There is a prerequisite that a customer has bought (or enrolled in a trial version for) the DBaaS instances from ISV vendor MongoDB Atlas or Crunchy Bridge.

DBaaS project is developed and productized using iterative development processes to allow feedback from users, enable/help ISV develop the required functionality and quickly release those to users. Following sections are focussed on the service definition as planned for Alpha release of DbaaS.


***Common ways to setup and configure databases in container platforms***

Imagine if we need to deploy one or more services that needs to interact with a database, one of the simplest ways of getting Database available for us while deploying in OpenShift would like something like below 

***Shell Script***

![Deploy Database ](dbaas-guide/documentation/modules/ROOT/assets/images/db1.png)

![Deploy Database Continued .... ](dbaas-guide/documentation/modules/ROOT/assets/images/db2.png)


***A better approach to Databases***

By using Managed Databases in the cloud, we can overcome need to provision databases within the same cluster where applications are deployed , however they still come with a set of additional challenges to deal with ...

Using Database services in the cloud but we still will have to deal with the problem of connecting the databases to applications while deployed in a container platform and some of the key challenges can be listed below 

***Challenges for ad hoc DBaaS in the Enterprise***

![Adhoc DB ](dbaas-guide/documentation/modules/ROOT/assets/images/challenge1.png )


Finally, BEST approach to provide a frictionless experience to Developers and Operations teammates can be described as below

***Red Hat OpenShift Database Access (RHODA)***

- Faster and easier self-service for developers
- More efficient connection, DB utilization
- Centralized monitoring, consistent control plane for admins

![RHODA ](dbaas-guide/documentation/modules/ROOT/assets/images/solution.png)


***How to***
This workshop can help deploy microservices using the managed databases supported by RHODA Operator