
For creating `Tanzu CommunityEdition(TCE)` managemet and workload cluster on a vSphere Homelab, see this previous [demo](https://github.com/pksheldon4/tce-on-vsphere-homelab).

However, this quick demonstration on using `CustomerResourceTemplates` can be used with any Tanzu Management Cluster.

The idea here is to create a Template to install common resources on all workload clusters created using the Tanzu CLI and a workload-cluster.yaml config file.

In this example, I will install the TCE Package Repository,  the `cert-manager` package,the `Contour` Ingress Controller pacakge and a custom imgpkg build of `metallb`.  You can follow this same strategy to install any resources into all workload clusters created after the template is applied to the management cluster.