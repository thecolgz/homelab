# TODO

- [Apply LXD VMs in parallel github.com/](../infra/Makefile#L12)
- [(optimize) DRY master and worker definition](../infra/cluster.tf#L89)
- [(bug) should be posible to put it in the profile instead lxd_profile.kubenode.config, and make it a variable](../infra/cluster.tf#L100)
- [use ./values/metallb.yaml for this](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L12)
- [(optimize) should cert manager be part of bootstrap?](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L33)
- [use ./values/cert-manager.yaml for this](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L43)
- [move Vault out of bootstrap](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L80)
- [upgrade vault helm version](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L85)
- [HA Vault](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L91)
- [Auto unseal Vault](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L92)
- [automatic ingress and tunnel for all services](../infra/modules/kubernetes-cluster-bootstrap/main.tf#L95)
- [Upgrade hosts kernel to use Wireguard in container](../infra/modules/vpn/main.tf#L15)
- [make parent interface a variable](../infra/modules/vpn/main.tf#L38)
- [Generate endpoint automatically (terragrunt for variable)](../infra/terraform.tf#L2)
- [convert to YAML for Terraform yamldecode](../metal/hosts.ini#L1)
- [Optimize SELinux](../metal/roles/lxd/tasks/main.yml#L1)
- [Optimize firewall](../metal/roles/lxd/tasks/main.yml#L6)
- [change to /var/lib/lxd/server.crt after https](../metal/roles/lxd/tasks/main.yml#L26)
- [(optimize) use template for tfvars](../metal/roles/lxd/tasks/main.yml#L38)
- [use btrfs in k8s 1.19.8 https](../metal/roles/lxd/templates/leader.yaml.j2#L17)
- [enable etcd authentication and generate terraform backend config variables](../metal/roles/tfstate/tasks/main.yml#L43)
- [investigate why --noconfirm is not working](../tools/Dockerfile#L3)