---
api_specs:
- filename: tensordock-instances-api-openapi.yml
  format: yaml
  label: TensorDock Instances API
  slug: tensordock-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-instances-api-openapi.yml
- filename: tensordock-secrets-api-openapi.yml
  format: yaml
  label: TensorDock Secrets API
  slug: tensordock-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-secrets-api-openapi.yml
- filename: tensordock-authorization-api-openapi.yml
  format: yaml
  label: TensorDock Authorization API
  slug: tensordock-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-authorization-api-openapi.yml
- filename: tensordock-billing-api-openapi.yml
  format: yaml
  label: TensorDock Billing API
  slug: tensordock-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-billing-api-openapi.yml
- filename: tensordock-containers-api-openapi.yml
  format: yaml
  label: TensorDock Containers API
  slug: tensordock-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-containers-api-openapi.yml
- filename: tensordock-hostnodes-api-openapi.yml
  format: yaml
  label: TensorDock Hostnodes API
  slug: tensordock-hostnodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-hostnodes-api-openapi.yml
- filename: tensordock-instant-vms-api-openapi.yml
  format: yaml
  label: TensorDock Instant VMs API
  slug: tensordock-instant-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-instant-vms-api-openapi.yml
- filename: tensordock-spot-api-openapi.yml
  format: yaml
  label: TensorDock Spot API
  slug: tensordock-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-spot-api-openapi.yml
- filename: tensordock-virtual-machines-api-openapi.yml
  format: yaml
  label: TensorDock Virtual Machines API
  slug: tensordock-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/openapi/tensordock-virtual-machines-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tensordock.com
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Aug 23 11:13:34 2026 GMT
  host: www.tensordock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: documenter.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:53:29 2026 GMT
  host: dashboard.tensordock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tensordock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TensorDock, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TensorDock
provider_slug: tensordock
slug: tensordock-domain-security
source_filename: tensordock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tensordock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documenter.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.tensordock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:53:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tensordock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensordock/refs/heads/main/security/tensordock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPU
- Cloud
- Marketplace
- Compute
- Virtual Machines
- AI
- Machine Learning
- Bare Metal
- Spot Instances
- Containers
---
