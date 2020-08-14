# eks-aws-cluster

Description how to create cluster on Amazon

*First of all we need 3 application to go that.

AWS CLI - needs for authentication and to run a commands
KUBECTL - for management k8s clusters
EKSCTL - for creating k8s clusters

*Then we are downloading packages and istalling programms on your machine or server.

*After that we are opening your Terminal and typing a command for a creating cluster on AWS. 
- eksctl create cluster --name(here we type a name of your cluster if we need a specific name, or it can be by default"

Here some commands to work with a cluster:

- kubectl cluster-info (for getting information about our cluster)
- kubectl cluster-info dump (for debugging and diagnosing problems)
- kubectl get nodes (for getting info about nodes(name,status,roles,ages,versions))
- kubectl delete cluster --name (for deleting a cluster)

*Also if we need a specific clusters, we can create them with a config files.

- eksctl create cluster -f (and a name of your config file, in your case it's @mycluster.yaml@)
- eksctl delete cluster -f mycluster.yaml
