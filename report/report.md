# Report for Lab4 AIT
### Authors: Mickael Bonjour & Miguel Gouveia
### Link to repository : https://github.com/mbonjour/Teaching-HEIGVD-AIT-2019-Labo-Docker

## Table of contents

## Introduction

## Task 0
### M1
Well not for the case described here. Because when people will connect in mass at Black Friday it will probably crash. And with this obscure bug that hasn't been fixed yet, the servers can crash without any charge. If it's the case nothing can restart the servers directly so there will be so awfully long downtimes.
### M2
We need to add a environment variable to the docker image of HAProxy (needed to know where the requests can be forwarded).That's done in the docker-compose.yml file in the environment section of ha image. And we need to add a web container to the docker-compose, the name of this container will be used by ha to forward the requests accordingly to the balancing strategy. So with these modifications we need to restart all the infrastructure and wait it's up to use it again.
### M3
We need a system where we can add/remove web servers and these can inform haproxy that they're here to respond to some HTTP requests. TO resolve the problem of crashing/overheating servers we need something to monitor the web servers and shutdowns/restart it when needed.
### M4
Like we said on M3, a system where the nodes inform the proxy of their presence and their capacities.
### M5 (TODO)
No we don't actually have the ability to perform these actions, maybe we can try with some shared volume where all the logs are created and one central container check the logs of all nodes and acts in consequences of the different logs seen.
### M6 (TODO)
### Image of the nodes
![Nodes proof](../assets/img/nodesProof.png)
### URL Repository
https://github.com/mbonjour/Teaching-HEIGVD-AIT-2019-Labo-Docker
## Task 1
### Image
The screenshot asked for in deliverables :
![Proof nodes are running](./assets/img/nodesProofTask1.png)

And in this image we can well see the s6 init who start the processes :
![Proof S6 working](./assets/img/proofStartS6.png)

### Difficulties and resume (TODO: need to be more specified)
We didn't have any difficulties doing this task. This task is made to implement the s6 processor supervisor. This supervisor will permit to run multiple processes in a container and don't stop it when the main process stop. That will maybe permit us to restart a process when it stops with s6 supervisor. 
## Task 2
### Configuration for serf process to s6 (both images)
![Adding Serf](./assets/img/s6AddSerf)
## TODO : We didn't had any problem with networking, aybe we need to use docker run command because I used docker-compose each time and it worked fine for me.

### Logs
See the Task2 folder in the logs folder.
### Answer to given problematic of misconception (TODO)
I don't see where the misconception resides at this point ?!?
It seems that is a problem with an uptime ofserver because it say that the replay option will not be helpful because of the misconception.

### Serf and others

## Task 3

## Task 4

## Task 5

## Task 6

## Difficulties

## Conclusion
