# eks-alb-ingress-controller

![alb-ingress](https://github.com/user-attachments/assets/5e139245-0835-4346-8acc-ebd0d3f248d5)

### Associates an OIDC provider with your EKS cluster

 - Associates an OIDC provider with your EKS cluster
 - Allows IAM roles to be used inside the Kubernetes cluster.

```
eksctl utils associate-iam-oidc-provider --cluster alb-demo-cluster  --approve --region us-east-2
```
# Step 1: Create IAM Role using eksctl

### Download an IAM policy for the AWS Load Balancer Controller that allows it to make calls to AWS APIs.
 
  - Since the AWS Load Balancer Controller needs permissions to manage AWS Load Balancers, you need to create an IAM policy and associate it     with a Kubernetes service account.

```
curl -O https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.11.0/docs/install/iam_policy.json
```
