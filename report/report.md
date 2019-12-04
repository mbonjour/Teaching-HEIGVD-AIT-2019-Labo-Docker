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
![Proof nodes are running](./assets/img/nodesProofTask1.png)

## Task 2

## Task 3

## Task 4

## Task 5

## Task 6

## Difficulties

## Conclusion
