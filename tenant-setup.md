## Multi-Tenancy Architecture in Kubernetes ##

**Concept of multi tenancy**: In kubernetets, multi-tenancy is when multiple users share a single cluster.

I have set up this on my own k8s cluster created in virtual box. Taken one master node and one worker node.

**Master Node IP: 192.168.1.50**            
`2 CPU & 4GB RAM`

**Worker Node IP: 192.168.1.53**            
`3 CPU & 4GB RAM`

![Virualbox](cluster-resources/images/vbox-home.png)

I have taken Centos7 Image to create these two VMs, Also installed & configured kubernetes latest 1.25 version using `kubeadm`.

![Virualbox](cluster-resources/images/cluster-info.png)

