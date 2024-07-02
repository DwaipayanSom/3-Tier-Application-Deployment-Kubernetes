Description: Implemented a three-tier architecture for deploying a web application using AWS and Kubernetes. The project involved setting up the Presentation, Logical, and Data Layers, and automating the deployment process using Kubernetes and various AWS services.

Key Contributions:

1. Presentation Layer (Tier 1): 
   - Containerized the frontend application.
   - Deployed frontend container on AWS Elastic Container Registry (ECR) and managed it using Kubernetes.

2. Logical Layer (Tier 2):
   - Containerized the backend application.
   - Deployed backend container on AWS ECR and managed it using Kubernetes.
   - Implemented business logic to handle user interactions and process data.

3. Data Layer (Tier 3):
   - Set up a MongoDB database to store and retrieve application data.
   - Managed database deployment and scaling using Kubernetes.

Deployment Steps:
1. Infrastructure Setup:
   - Created IAM user and configured AWS CLI for access management.
   - Launched and configured EC2 instances as the base infrastructure.
   
2. Containerization:
   - Built Docker images for frontend and backend applications.
   - Pushed images to AWS ECR for centralized management.
   
3. Kubernetes Setup:
   - Created an Amazon EKS cluster and configured it for managing the application containers.
   - Deployed the application using Kubernetes manifests for deployments and services.
   
4. Load Balancing and Ingress:
   - Configured AWS Application Load Balancer for external traffic management.
   - Set up Kubernetes Ingress for internal routing between frontend, backend, and database tiers.
   
5. Automation and Management:
   - Used Helm for managing Kubernetes packages and deploying the load balancer controller.
   - Automated the creation and destruction of the infrastructure using AWS CloudFormation.

Technologies Used: AWS (EC2, ECR, EKS, IAM, CloudFormation, CodePipeline, CodeBUild), Kubernetes, Docker, Helm, MongoDB

Outcome: Successfully deployed a scalable and resilient three-tier web application architecture, ensuring efficient interaction between user interface, business logic, and data storage layers.
