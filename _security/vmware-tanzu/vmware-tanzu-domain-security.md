---
api_specs:
- filename: vmware-tanzu-service-mesh-openapi.yml
  format: yaml
  label: VMware Tanzu Service Mesh API
  slug: tanzu-service-mesh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/openapi/vmware-tanzu-service-mesh-openapi.yml
- filename: vmware-tanzu-kubernetes-grid-openapi.yml
  format: yaml
  label: VMware Tanzu Kubernetes Grid API
  slug: tanzu-kubernetes-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/openapi/vmware-tanzu-kubernetes-grid-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vmware.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: tanzu.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: docs.vmware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: prod-2.nsxservicemesh.vmware.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vmware Tanzu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VMware Tanzu, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VMware Tanzu
provider_slug: vmware-tanzu
slug: vmware-tanzu-domain-security
source_filename: vmware-tanzu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tanzu.vmware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vmware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: prod-2.nsxservicemesh.vmware.com\n  https: false\ndomains:\n- domain: vmware.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/security/vmware-tanzu-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud Native
- Containers
- Enterprise
- Kubernetes
- Multi-Cloud
- Service Mesh
- VMware
---
