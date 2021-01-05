# Cert-Manager

cert-manager is a Kubernetes add-on to automate the management and issuance of TLS certificates from various issuing sources.

It will ensure certificates are valid and up to date periodically, and attempt to renew certificates at an appropriate time before expiry.

# How does it work?

Cert-manager automates the DNS-01 challenge by putting a specific value in a TXT record under the domain name.
It would need access a gcloud service account with access to cloud dns to be able to create the TXT record.

## How to use a certificate

- Ensure a cluster issuer has been setup
- Create a certificate secret in the corresponding namespace
- Ensure traefik uses the tls secret

## Links
- https://letsencrypt.org/docs/challenge-types/#dns-01-challenge
- https://github.com/jetstack/cert-manager
- https://cert-manager.io/docs/installation/kubernetes/
- https://github.com/jetstack/cert-manager/releases/download/v1.1.0/cert-manager.yaml
