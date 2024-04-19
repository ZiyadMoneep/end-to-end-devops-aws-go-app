# End-to-end-DevOps | Go Application

This repository contains scripts and Kubernetes manifests for deploying the Go application on an AWS EKS cluster with an accompanying ECR repository and EBS volumes. The deployment includes setting up an Ingress controller, monitoring with Prometheus and Grafana, and a continuous deployment pipeline.

## Before you run the script

### Update Script Variables:

The `build.sh` script contains a set of variables that you need to customize according to your AWS environment and deployment requirements. Here's how you can update them:

1. Open the `build.sh` script in a text editor of your choice.

2. Update the variables at the top of the script with your specific configurations:

   ```bash
   cluster_name="YOUR_EKS_CLUSTER_NAME"
   region="YOUR_AWS_REGION"
   aws_id="YOUR_AWS_ACCOUNT_ID"
   repo_name="YOUR_REPO_NAME"
   domain="YOUR_DOMAIN.com"
   namespace="go-survey"
   ```

3. Save the changes to the `build.sh` script.
