cka 2022 1.22

CKA Curriculum

25% - Cluster Architecture, Installation & Configuration
- [ ] Alias and completion
- [ ] Manage role based access control (RBAC)
- [ ] Use Kubeadm to install a basic cluster
  - [x] install kubeadm https://kubernetes.io/fr/docs/setup/production-environment/tools/kubeadm/install-kubeadm/#installation-de-kubeadm-des-kubelets-et-de-kubectl
  - [x] possibility to fix version `apt install -y kubeadm=1.21.1-00 kubelet=1.21.1-00 kubectl=1.21.1-00`
  - [x] install docker `apt install docker.io` `<3`
  - [x] verify cgroupfs driver ` sudo docker info | grep -i cgroup  ` else change cgroupfs for docker /etc/docker/daemon.json `{ "exec-opts": ["native.cgroupdriver=systemd"] }` `<3`
  - [x] kubeadm init --pod-network-cidr 192.168.0.0/16
  - [x] install cni example calilco in 3.22 ! https://kubernetes.io/fr/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/#pod-network
  - [ ] join to cluster https://kubernetes.io/fr/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/#join-nodes
  - [x] remove taints for execute workload pods on master `kubectl taint nodes --all node-role.kubernetes.io/master-`
- [ ] Manage a highly-available Kubernetes cluster
- [ ] Provision underlying infrastructure to deploy a Kubernetes cluster
- [x] [ ] Perform a version upgrade on a Kubernetes cluster using Kubeadm https://kubernetes.io/docs/tasks/administer-cluster/kubeadm/kubeadm-upgrade
- [x] [ ] Implement etcd backup and restore https://kubernetes.io/fr/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/#isolation-des-n%C5%93uds-du-control-plane

15% - Workloads & Scheduling
- [ ] Understand deployments and how to perform rolling update and rollbacks
- [ ] Use ConfigMaps and Secrets to configure applications [x]
- [ ] Know how to scale applications
- [ ] Understand the primitives used to create robust, self-healing, application deployments
- [ ] Understand how resource limits can affect Pod scheduling
- [ ] Awareness of manifest management and common templating tools

20% - Services & Networking
- [ ] Understand host networking configuration on the cluster nodes
- [ ] Understand connectivity between Pods
- [ ] Understand ClusterIP, NodePort, LoadBalancer service types and endpoints
- [ ] Know how to use Ingress controllers and Ingress resources
- [ ] Know how to configure and use CoreDNS
- [ ] Choose an appropriate container network interface plugin

10% - Storage
- [ ] Understand storage classes, persistent volumes
- [ ] Understand volume mode, access modes and reclaim policies for volumes
- [ ] Understand persistent volume claims primitive
- [ ] Know how to configure applications with persistent storage

30% - Troubleshooting
- [ ] Evaluate cluster and node logging
- [ ] Understand how to monitor applications
- [ ] Manage container stdout & stderr logs
- [ ] Troubleshoot application failure
- [ ] Troubleshoot cluster component failure
- [ ] Troubleshoot networking
