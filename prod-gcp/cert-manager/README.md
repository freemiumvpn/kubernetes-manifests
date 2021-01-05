# Cert-Manager

cert-manager is a Kubernetes add-on to automate the management and issuance of TLS certificates from various issuing sources.

It will ensure certificates are valid and up to date periodically, and attempt to renew certificates at an appropriate time before expiry.

## How to use a certificate

- Ensure a cluster issuer has been setup
- Create a certificate secret in the corresponding namespace
- Ensure traefik uses the tls secret

## Links

- https://github.com/jetstack/cert-manager
- https://cert-manager.io/docs/installation/kubernetes/
- https://github.com/jetstack/cert-manager/releases/download/v1.1.0/cert-manager.yaml
