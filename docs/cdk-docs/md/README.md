# Scenario Index

* Scenario 1 - [Moving existing apps to the cloud](01-moving-existing-apps.md)

* Scenario 2 - [A Developer Introduction to OpenShift](02-developer-intro.md)

* Scenario 3 - [Transforming an existing monolith (Part 1)](03-mono-to-micro-part-1.md)

* Scenario 4 - [Transforming an existing monolith (Part 2)](04-mono-to-micro-part-2.md)

* Scenario 5 - [Building Reactive Microservices](05-reactive-microservices.md)

* Scenario 6 - [Prevent and detect issues in a distributed system](06-resilient-apps.md)

# Monoliths to Microservices: App Transformation Hands-on Workshop



 These documents contains a complete set of instructions for running the workshop, split into different _scenarios_. You can use these documents as a companion as you progress through the scenarios, but keep in mind that some of the links in this document may not work as they will be specific to your online environment. You will be expected to substitute your own values for the following URLs:

 * **$OPENSHIFT_MASTER** - When you see this variable, replace it with the value of your own OpenShift master hostname/port, such as `https://master.openshift.com:8443` (be sure to include the port!).

 * **$ROUTE_SUFFIX** - When you see this variable, replace it with the value of your own OpenShift default routing suffix. For example, if you see `http://coolstore-dev.$ROUTE_SUFFIX` then you would replace this with `http://coolstore-dev.apps.mycompany.com` assuming your OpenShift cluster uses a default routing suffix of `apps.mycompany.com`.

# Intro

As modern application requirements become more complex, it’s apparent that one runtime, one
framework, or one architectural style is no longer a feasible strategy. Organizations must figure out how
to manage the complexity of distributed app development with diverse technologies, a lack of skilled
resources, and siloed processes.

In this hands-on workshop you’ll learn about:

* Migrating an existing legacy Java™ EE app to [Red Hat JBoss
Enterprise Application Platform](https://developers.redhat.com/products/eap/overview/) on [OpenShift](https://developers.redhat.com/products/openshift/overview/).
* Using modern frameworks like [Spring Boot](https://projects.spring.io/spring-boot/), [Wildfly Swarm](http://wildfly-swarm.io),
[Eclipse Vert.x](http://vertx.io), and [Node.js](https://nodejs.org) to implement microservices and
replace monolithic functionality.
* Developing and deploying using [Red Hat OpenShift Container
Platform](https://developers.redhat.com/products/openshift/overview/), [Red Hat OpenShift Application Runtimes](https://developers.redhat.com/products/rhoar/overview/), and
DevOps processes.
* The benefits and challenges with microservices, including use
cases for reactive microservices.
* Preventing and detecting issues in a distributed system.
* API gateways and microservices.

# Accessing the lab and verifying pre-requisites

You can register for the lab by using the url provided by the instructor.
Once you have registered for the lab you will get the lab environment details. Using the given credentials, login to **Azure** and ensure that you can access the resource groups created. Then open the resource group and **SSH** into the **LABVM (jump-VM)**, give **root permissions to the user** and continue with the lab. 
* Verify the pre-requisites by running the following commands
  *	**git --version** (it should be 2.7.2 or later)
  *	**java -version** (it should be 1.8.x or later)
  *	**oc** (ensure that this command is working, if not it will show Command not found.)
  *	**mvn --version** (it should be 3.3.9 or later)
  * navigate to **/root** and ensure that **Projects, rhamt-cli-4.0.0.Beta4 and jboss-eap-7.1.0.zip** folders are already present.






