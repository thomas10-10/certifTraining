cka 2022 1.22

CKA Curriculum

25% - Cluster Architecture, Installation & Configuration
- [ ] Manage role based access control (RBAC)
- [ ] Use Kubeadm to install a basic cluster
  - install kubeadm https://kubernetes.io/fr/docs/setup/production-environment/tools/kubeadm/install-kubeadm/#installation-de-kubeadm-des-kubelets-et-de-kubectl
  - possibility to fix version
  - install docker `apt install docker.io`
  - verify cgroupfs driver ` sudo docker info | grep -i cgroup  ` else change cgroupfs for docker /etc/docker/daemon.json '{ "exec-opts": ["native.cgroupdriver=systemd"] }'
  - kubeadm init --pod-network-cidr 192.168.0.0/16
  - install cni example calilco in 3.22 ! https://kubernetes.io/fr/docs/setup/production-environment/tools/kubeadm/create-cluster-kubeadm/#pod-network
- [ ] Manage a highly-available Kubernetes cluster
- [ ] Provision underlying infrastructure to deploy a Kubernetes cluster
- [ ] Perform a version upgrade on a Kubernetes cluster using Kubeadm
- [ ] Implement etcd backup and restore
- [ ] Understand deployments and how to perform rolling update and rollbacks
- [ ] Use ConfigMaps and Secrets to configure applications
- [ ] Know how to scale applications
- [ ] Understand the primitives used to create robust, self-healing, application deployments
- [ ] Understand how resource limits can affect Pod scheduling
- [ ] Awareness of manifest management and common templating tools
