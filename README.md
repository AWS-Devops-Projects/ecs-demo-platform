# Amazon ECS Workshop


This is part of an Amazon ECS workshop at https://ecsworkshop.com


## DEPLOYING MICROSERVICES TO ECS

https://ecsworkshop.com/images/3-tier-architecture.svg



## CONFIGURE CLOUDWATCH CONTAINER INSIGHTS FOR YOUR ECS CLUSTER


You can use CloudWatch Container Insights to collect, aggregate, and summarize metrics and logs from your containerized applications and microservices. Container Insights is available for Amazon Elastic Container Service, Amazon Elastic Kubernetes Service, and Kubernetes platforms on Amazon EC2. The metrics include utilization for resources such as CPU, memory, disk, and network. Container Insights also provides diagnostic information, such as container restart failures, to help you isolate issues and resolve them quickly.

## AMAZON ECS CLUSTER CAPACITY PROVIDERS

 how Capacity Providers can help us in managing autoscaling for EC2 backed tasks, as well as ways to implement cost savings when running Fargate tasks. We will implement two capacity provider strategies in our cluster:

For a Fargate backed ECS service, we will implement a strategy to deploy that service as a mix between Fargate and Fargate Spot.

For an EC2 backed ECS service, we will implement Cluster Auto Scaling by increasing the task count of a service beyond the capacity available. This will require the backend EC2 infrastucture to scale to meet the demand, which the ECS cluster autoscaler will handle.

## BLUE/GREEN DEPLOYMENTS ON ECS FARGATE


Blue/Green deployment is a technique for releasing an application by shifting the traffic between two identical environments running different versions of the same application. Blue/Green deployment is recommended for critical workloads since it mitigates the risks associated with deploying software, such as downtime and rollback capability.

Traditionally, with in-place upgrades, it was difficult to validate your new application version in a production deployment while also continuing to run your old version of the application. After you deploy the green environment, you have the opportunity to validate it. If you discover the green environment is not operating as expected, there is no impact on the blue environment. You can route traffic back to it, minimizing impaired operation or downtime, and limiting the blast radius of impact.

## STATEFUL WORKLOADS ON ECS FARGATE

we will deploy a stateful workload on ECS Fargate with storage persisting on EFS. There are many reasons for wanting to deploy a stateful workload on containers, with some examples being:

Content Management Systems like Wordpress, or Drupal.
Sharing static content for web servers
Jenkins Master Nodes
Machine learning
Relational Databases for dev/test environments

## LOCAL TESTING USING THE ECS-CLI


MORE RESOURCES
Discover more AWS resources for building and running your application on AWS:

Containers from the Couch - Check out our latest container shows, and learn all about running containers!
More Workshops
Amazon EKS Workshop - This workshop guides you through the process of setting up and using a Kubernetes cluster on AWS
Amazon Lightsail Workshop - If you are getting started with the cloud and looking for a way to run an extremely low cost environment Lightsail is perfect. Learn how to deploy to Amazon Lightsail with this workshop.
Tools for AWS Fargate and Amazon ECS
Containers on AWS - Learn common best-practices for running containers on AWS
copilot-cli - The AWS Copilot CLI is a tool for developers to create, release and manage production ready containerized applications on Amazon ECS and AWS Fargate.
fargate - Command line tool for interacting with AWS Fargate. With just a single command you can build, push, and launch your container in Fargate, orchestrated by ECS.
Terraform - Use Terraform to deploy your docker containers in Fargate
Wonqa is a tool for spinning up disposable QA environments in AWS Fargate, with SSL enabled by Let’s Encrypt. More details about Wonqa on the Wonder Engineering blog
coldbrew - Fantastic tool that provisions ECS infrastructure, builds and deploys your container, and connects your services to an application load balancer automatically. Has a great developer experience for day to day use
mu - Automates everything relating to ECS devops and CI/CD. This framework lets you write a simple metadata file and it constructs all the infrastructure you need so that you can deploy to ECS by simply pushing to your Git repo.
Courses
Microservices with Docker, Flask, and React - Learn how to build, test, and deploy microservices powered by Docker, Flask, React Amazon ECS!


