# Streamlining Chaos: AsciiArtify's Journey with Terraform and Argo CD

## The Challenge

The AsciiArtify team, in their rush to innovate, deployed an expansive suite of services on GCP using Terraform. This rapid growth resulted in a complex web of deployments that became difficult to manage.

## The Arrival

As an experienced DevOps professional, I was tasked with organizing this chaos. My goal was clear: implement a system that could manage these deployments efficiently and maintain order.

## The Solution

I chose Argo CD, a tool designed for managing deployments using GitOps principles. This would allow us to define our infrastructure and application configurations as code in Git, providing a single source of truth for our deployments.

## Implementation

1. **Cataloging Resources**: I started by identifying and categorizing all existing deployments. 

2. **Helmify** I introduced the team to [Helmify](https://github.com/arttor/helmify), a tool that automates the creation of Helm charts from existing Kubernetes objects. This addition was crucial in streamlining our deployment processes and enhancing our use of GitOps.

![Install Minikube and deploy](https://github.com/diamonce/AsciiArtify/blob/main/argocd.gif?raw=true)
<img src="![Install Minikube and deploy](https://github.com/diamonce/AsciiArtify/blob/main/argocd.gif?raw=true)">

3. **Deploying Argo CD with Helm charts**: Argo CD was set up within our Kubernetes clusters, connected to our Git repositories. This setup enabled automatic synchronization of our deployments with the configurations defined in Git.

![Terraform deployments are now in Argocd](https://raw.githubusercontent.com/diamonce/AsciiArtify/main/doc/argo1.png)
<img src="![Terraform deployments are now in Argocd](https://raw.githubusercontent.com/diamonce/AsciiArtify/main/doc/argo1.png)">

![Terraform deployments are now in Argocd](https://raw.githubusercontent.com/diamonce/AsciiArtify/main/doc/argo2.png)
<img src="![Terraform deployments are now in Argocd](https://raw.githubusercontent.com/diamonce/AsciiArtify/main/doc/argo2.png)">

## The Outcome

Through the implementation of Argo CD and the refinement of our Terraform configurations, we achieved a manageable and scalable infrastructure. Deployments became streamlined, and the team gained confidence in managing and scaling our cloud environment.
