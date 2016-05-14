---
---
<!--- master only -->
> ![warning](../../images/warning.png) This document applies to the HEAD of the calico-containers source tree.
>
> View the calico-containers documentation for the latest release [here](https://github.com/projectcalico/calico-containers/blob/v0.19.0/index).
<!--- else
> You are viewing the calico-containers documentation for release **release**.
<!--- end of master only -->

# Kubernetes with Calico networking
Calico can be used as a network plugin for Kubernetes using the Container Network Interface to provide connectivity for workloads in a Kubernetes cluster.  Calico is particularly suitable for large Kubernetes deployments on bare metal or private clouds, where the performance and complexity costs of overlay networks can become significant. It can also be used in public clouds.

To start using Calico Networking in your existing Kubernetes cluster, check out our [integration tutorial](KubernetesIntegration).

To build a new Kubernetes cluster with Calico networking, try one of the following guides:

Quick-start guides:
- [CoreOS Vagrant](VagrantCoreOS)
- [CoreOS on GCE](GCE)
- [CoreOS on AWS](AWS)
- [Docker Compose](https://github.com/projectcalico/docker-compose-kubernetes) 

Bare-metal guides:
- [CoreOS bare-metal](https://github.com/kubernetes/kubernetes/blob/master/docs/getting-started-guides/coreos/bare_metal_calico)
- [Ubuntu bare-metal](https://github.com/kubernetes/kubernetes/blob/master/docs/getting-started-guides/ubuntu-calico)

# Kubernetes with Calico policy
Calico can provide network policy for Kubernetes clusters using the v1alpha1 Kubernetes network-policy API.

This feature is currently in alpha and disabled by default.  The following guide explains how to enable and use Calico policy on Kubernetes. 
- [Kubernetes v1alpha1 Network Policy](NetworkPolicy)

Calico also supports network policy using annotaions.  This method is deprecated, and as such is not recommended.
- [Calico policy using Annotations](AnnotationPolicy) [Deprecated]

# Requirements
- The kube-proxy must be started in `iptables` proxy mode.

# Troubleshooting 
- [Troubleshooting](Troubleshooting)

[![Analytics](https://calico-ga-beacon.appspot.com/UA-52125893-3/calico-containers/docs/cni/kubernetes/index?pixel)](https://github.com/igrigorik/ga-beacon)
