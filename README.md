# Kubernetes cluster on AWS created using kops

## Deploy a cluster builder and subsequent 2 nodes Kubernetes cluster within a VPC with 2 subnets

The template (parent-template.yaml) deploys a Kops Linux EC2 instance to create kubernetes cluster with 2 worker nodes (t2.micro) and 1 master node (t2.medium) on the new VPC. NAT gateway is also deployed to enable internet connectivity for the Kops Linux EC2 instance

[![cloudformation-launch-stack](assets/stack-launch.png)](https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-2#/stacks/new?stackName=Cluster-Builder&templateURL=http://cybersociety.s3.amazonaws.com/cf-templates/parent-template.yaml)

## Deploy the CodePipeline

The template (CodePipeline.yaml) deploys a AWS CodePipeline connected to your own GitHub repository. In this template, forked Repo <https://github.com/hyperionian/ecs-demo-php-simple-app> is used as a source for the pipeline.

[![cloudformation-launch-stack](assets/stack-launch.png)](https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-2#/stacks/new?stackName=CodePipeline&templateURL=http://cybersociety.s3.amazonaws.com/cf-templates/CodePipeline.yaml)
