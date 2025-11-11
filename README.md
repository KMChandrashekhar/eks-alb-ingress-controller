# eks-alb-ingress-controller

![alb-ingress](https://github.com/user-attachments/assets/5e139245-0835-4346-8acc-ebd0d3f248d5)

### Associates an OIDC provider with your EKS cluster

 - Associates an OIDC provider with your EKS cluster
 - Allows IAM roles to be used inside the Kubernetes cluster.

```
eksctl utils associate-iam-oidc-provider --cluster alb-demo-cluster  --approve --region us-east-2
```

