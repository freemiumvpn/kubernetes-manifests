# External DNS

ExternalDNS makes Kubernetes resources discoverable via public DNS servers. It retrieves a list of resources (Services, Ingresses, etc.) from the Kubernetes API to determine a desired list of DNS records.

## How does it work?

ExternalDNS allows you to control DNS records dynamically via Kubernetes resources in a DNS provider-agnostic way.
It would need access a gcloud service account with access to cloud dns to be able to create CNAME records.

## Links
- https://github.com/kubernetes-sigs/external-dns
- https://github.com/kubernetes-sigs/external-dns/blob/master/docs/tutorials/hostport.md#manifest-for-clusters-with-rbac-enabled
- https://github.com/kubernetes-sigs/external-dns/blob/master/docs/tutorials/gke.md
