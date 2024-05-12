# DevOps-Engineer-Challenge

Step 1: Docker

Build a Dockerfile for deploying a simple Ruby on Rails application with PostgreSQL DB enabled. Application and DB should run on different containers.

Step 2: Kubernetes

Build a YAML file for the same application you’ve used in your first step to deploy it on Kubernetes. You can use any local cluster provider such as Minikube or K3d. The deployment of the standalone PostgreSQL pod must use Kubernetes StatefulSet. Additionally, the candidate may use any ingress controller they are comfortable with or a service mesh.

Useful Documentation: Ingress Nginx Deployment

Step 3: ArgoCD

Deploy ArgoCD to manage the deployment of the previously mentioned application using GitOps. The candidate must create a private GitHub repository to manage the YAML files and for GitOps purposes. All ArgoCD config files must be present in the GitHub repository. The expected files include application.yaml to define the application to deploy, ArgoCD config maps (argocd-cm and argocd-rbac-cm), a config file for/(to add) the private GitHub repository and Kubernetes manifest files.

Useful Documentation: ArgoCD Documentation

Step 4: Tekton

Set up Tekton pipelines and the Tekton dashboard. The pipeline should download the source code from the public fork of the sample project (Which you’ve containerized in the first step), build the image, and push it to Docker Hub. The candidate is expected to manually run the pipeline from the Tekton dashboard.

Useful Documentation:

Tekton Documentation
Tekton Dashboard Documentation
Kaniko Task Documentation