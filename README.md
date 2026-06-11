## Kubernetes Deployment and Autoscaling on Amazon EKS

**Scenario:**

ShopEase is a growing e-commerce company that's getting ready to modernize the way its backend services run. The engineering team wants to nail down a consistent, repeatable way to package and deploy applications before going all-in on microservices at scale.
Right now, the backend service is:
•	Running locally on individual machines during development
•	Being packaged and started manually every single time
•	Behaving differently across machines — what works on one doesn't always work on another
•	Running with no orchestration platform watching over it
As the team gears up for future growth, they need a deployment model that's reliable, repeatable, and works the same way regardless of where it runs. One that can also scale when traffic picks up.
That's why the decision was made to move the service to Kubernetes — specifically Amazon Elastic Kubernetes Service (EKS) — to handle container management, deployments, and networking.



## My Role as the DevOps Engineer:

My job was to take this backend application and deploy it the cloud-native way using Kubernetes.
I was responsible for:
•	Packaging the application as a Docker container
•	Storing the image in a container registry
•	Running the application on a managed Kubernetes cluster
•	Exposing the service so it can be accessed from outside
•	Understanding how Kubernetes actually manages Pods and routes traffic



## Solution:

I deployed a containerized backend service on Amazon EKS and let Kubernetes take care of managing it.
The solution includes:
•	A Dockerized application stored in Amazon ECR
•	An Amazon EKS cluster with EC2 worker nodes
•	A Kubernetes Deployment to run and manage Pods
•	A Kubernetes Service (NodePort) to expose the application externally
•	Health endpoints to verify the application is running correctly
The focus of this project is on getting comfortable with Kubernetes fundamentals — not production-grade optimizations. Things like HTTPS, Ingress, and autoscaling are intentionally left for later projects.



## About the Project:

In this hands-on project, I be deployed a real backend service on Kubernetes and actually understanding how it runs inside an EKS cluster.

By the end, I have learned:
•	How application code gets turned into a Docker image
•	How Kubernetes pulls images from a registry
•	How Deployments create and manage Pods
•	How Services route traffic to the right Pods
•	How AWS networking and security groups tie into all of this
The application has API endpoints, health checks, and a simple UI to observe what's happening at runtime.
The goal is for Kubernetes to feel practical and logical by the end — not abstract or confusing.



## Steps Followed:

1.	Understand Kubernetes and Amazon EKS concepts
2.	Containerize the application using Docker
3.	Push the Docker image to Amazon ECR
4.	Create an Amazon EKS cluster
5.	Deploy the application using a Kubernetes Deployment
6.	Expose the application using a Kubernetes Service (NodePort)



## Services used:

•	Docker — to containerize the application
•	Amazon ECR — to store the Docker images
•	Amazon EKS — the managed Kubernetes cluster
•	Amazon EC2 — the worker nodes that run inside the cluster
•	Amazon VPC — handles networking for EKS
•	AWS IAM — manages permissions and access control
•	Kubernetes (kubectl) — to deploy and manage workloads



## Architectural Diagram:

<img width="1059" height="558" alt="image" src="https://github.com/user-attachments/assets/d38f0955-5361-47df-996d-7aa7f662d1c8" />



## Final Result:

<img width="940" height="474" alt="image" src="https://github.com/user-attachments/assets/8a333712-863e-4d52-8515-d7c806cd5b51" />


