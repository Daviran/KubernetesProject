# KubernetesProject

A Kubernetes Project made during my course at Epitech. <br>
Goal of the project : Deploy an application to a multi-host cluster using Kubernetes, and use Traefik as a reverse proxy and load balancer.

## Specifications: 

There are five elements constituting the application:
- Poll, a Flask Python web application that gathers votes and push them into a Redis queue.
- A Redis queue, which holds the votes sent by the Poll application, awaiting for them to be consumed by
the Worker.
- The Worker, a Java application which consumes the votes being in the Redis queue, and stores them into
a PostgreSQL database.
- A PostgreSQL database, which (persistently) stores the votes stored by the Worker.
- Result, a Node.js web application that fetches the votes from the database and displays the. . . well, result.

So : define 1 load balancer, 2 databases and 3 services, two of which will be routed using Traefik. <br>
     define a monitoring tool to get information on your containers. (cadvisor)
     
## Environment:
- 1 Kubernetes master and 2 nodes (workers).
- Hosted on GKE 
