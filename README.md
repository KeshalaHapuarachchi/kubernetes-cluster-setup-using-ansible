# kubernetes-cluster-setup-using-ansible

**Kubernetes Cluster Setup in Public Cloud Using Ansible**

# Steps to run Ansible Playbook for setting Cluster in AWS

Ansible playbook is located in aws folder

Add the AWS instances IPs and ssh key path to aws-hosts file

Run the following commands:

     # check the ansible playbook syntax
     ansible-playbook --syntax-check kubernetes-cluster-1M-2W.yaml -i aws-hosts

     # run the playbook
     ansible-playbook kubernetes-cluster-1M-2W.yaml -i aws-hosts
     
The join command for worker nodes to join the master node is in the cluster-join.txt file created by kubeadm init command and is located in the home directory of your Master node

