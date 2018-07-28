# Kubernetes cluster on AWS created using kops.


### Deploy a cluster builder and subsequent 2 nodes kubernetes cluster within a VPC with 2 subnets
[![cloudformation-launch-stack](assets/stack-launch.png)](https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-2#/stacks/new?stackName=Cluster-Builder&templateURL=http://cybersociety.s3.amazonaws.com/cf-templates/parent-template.yaml)

### Deploy the CodePipeline
[![cloudformation-launch-stack](assets/stack-launch.png)](https://console.aws.amazon.com/cloudformation/home?region=ap-southeast-2#/stacks/new?stackName=CodePipeline&templateURL=http://cybersociety.s3.amazonaws.com/cf-templates/CodePipeline.yaml)

The template deploys a AWS CodePipeline with your own specified GitHub repository.
