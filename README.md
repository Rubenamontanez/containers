# containers

benefits of containers
agility, scalability/high availability, cost optimization, portability.
Common use cases would be a CI/CD automation, autoscaling microservices architectures, containers as a service, and hybrid cloud architectures.

Dont replace Vms
Containers are a way in which we can place and isolate data and applications in to a container that's able to move between places.

when to  you use containers? 
They're going to add cost. They're going to add complexity. And they're going to add some latency in development especially with your first and second tries at working with containers. 
Need when the ability to isolate applications for portability. The ability to isolate applications for performance as they exist in a cluster. The ability to simplify some development operations. 

However, if you're trying to get traditional operations systems moving to containers just for the fact that you like to move to containers, you may find that they're mismatched in some ways. And the application requirements really are not a good fit for containers. Keep in mind they do add cost and complexity. Thus, there should be a clear case

containers as a service, hybrid cloud architectures, application migration, and cost optimization.


What is an advantage of Containers?
Multiple operating systems and package versions function without the mess of conflicts and mismatches.
Containers use a layered approach.
Docker is the leader of the Container ecosystem.

 Advantages 
 - a truly distributed application that leverages components in isolation. That's what containers are.
 They provide us with a truly distributed application that leverages components and they're isolated so they can operate on their own.
 - if your refactoring your application anyways, then moving to containers is a good way to go
 - Portability can be exceptional, obviously, with containers, Allows nonportable applications to be protable and move from cloud to cloud and platform to platform. And we've had this before with, certainly, Java and J2EE People want to write to portability, however, there is a trade off that you may be missing some of the native features by writing applications, in this case containers that are portable. However, in Docker they've mapped that to the various native capabilities of the runtime operating system that sits in the platform so it's able to take advantage of the native features of the runtime platform even though you're writing to a portable layer of extraction.
- access to data is a bit tricky in containers. We have to deal with different security parameters, different tool sets, things are typically new. There are not a lot of people out there who know how to design

Disadvantages 
- They cost more than just lift and shift . 
- Its very complex in term of Devops, Alot of different factors need to sync and work together in order for it to work. Since its newer support isnt completely there. Althoug due to open source its getting better
-just because you can put them in containers doesnt mean you should.

Containerized Applications
- Designed from the ground up. Focus on what you will do with it not what it will be. Consider scaling and the size of your container. Understand what the target application needs to do 

Container design
- The Basics of Container Design. First, Understand the components.  we need to understand why containers exist and what are the mechanisms that exist within containers and how they're levered? When buiding an application they have to take advantage of the container-based infrastructure that's provided and that can be a bit complex but it's very important to understand all of the pieces. 
- Understand how they interoperate. How does containers communicate with data? How do they communicate with message cues? How they produce API's or microservices. All these things have to be understood and built within the system. 
- containers should never have a time limit set on their particular durability. 
- They're images which are read-only templates. Images are used to create Docker containers. So their templates are designers for what a Docker container is. A container is just nothing more of an instance of an image. They're a public or private stores from which you can upload or download images. So they're available for you to reuse. Containers are similar to a directory. A Docker container holds everything that is needed for an application to run 
- Registries are stateless, scalable server-side applications that stores and lets you distribute Docker images. Registries allow you to distribute Docker images, either locally, or over the open internet. Containers are instances of images and images are read-only templates. 
- A container image is to a container as a VM template is to a VM. So that allows you to understand that a container image is to a container as a VM template is to a VM. So an image actually is a template for a container and so an image, basically, defines what a container is and a container basically is an instance of an image.

Container Data
- Data needs to be persisted in Docker for most applications. So we have to figure out a mechanism in a way in which you're going to store the data, or else the data won't exist after the container is shut down. 
- One, is keeping your data persistent even though the container gets restarted. So we basically just write directly to the system and it's going to be persisted and it's going to endure itself from different restart to different restarts. It's very much like rebooting the containers.
- So you can actually store the data down on the host filesystem, and that will be of course present when the Docker container relaunches and it can just basically access the same filesytem.
- using the Docker data volume, you can share the data with other Docker containers. So it allows you to, in essence, set up a data sharing mechanism that allows different containers to communicate one to another, and share common data repository, in essence, a database.

Build Container
- So the build process is technical to understand. Often it's automated, so you don't necessarily have to keep memorizing the steps. However, it is helpful for you to understand how containers are built. So as tools progress, the process is likely to change as ways toi build get better

Deployments 
- You have to operate these containers for years and years, so think about the operational procedures, and how backup and recovery, and security, and all these sorts of things needs to fit into the correct operations of your container platform, in your container-based applications. Consider the Ops or operation in DevOps and how they will continue to improve.
- Orchestration is key to healthy container deployments and operations. So Kubernetes, Mesosphere, Docker Swarm, those things are in essence the environment in which they can run, where they can be managed as clusters of objects. Containers alone are nothing
- Have to be able to scale 

Common uses
Development and testing CI/CD
- doing continuous integration/continuous development on top of the Docker platform, you're able to achieve additional agility based on the fact that they're able to become more consistent and reduce the complexity of their environment.

Autoscaling microservices architectures.
- Capital One, a bank, they had an analytical garage that was able to provide new analytical container work flows, so they leverage a portal, they're able to use user authentication, they're able to do a container that picks what they're looking to do, initiate JSON, leverage a docker engine on the host instantiates container, leverages Mesos as their orchestrator, and they're able to leverage Marathon which is a third-party product. So Mesos and Marathon work
- Using different docker containers, they're able to multiplex and access the data to return the analytical component. This is an example of a data oriented docker application that's able to gain access to huge amounts of data, and call through that data to determine certain analytical data points that need to be externalized to people who are leveraging the containers. So in this case, the users in our portal are
