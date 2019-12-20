Using the efs-provisioner to automatically provision EFS PersistentVolumes

https://aws.amazon.com/premiumsupport/knowledge-center/eks-pods-efs/

1. `$ k apply -f class.yaml`

1. Update configmap.yaml with the correct `file.system.id` and `aws.region`

1. `$ k apply -f configmap.yaml`

1. `$ k apply -f rbac.yaml`

1. Update the nfs server value in deployment.yaml

1. `$ k apply -f deployment.yaml`
