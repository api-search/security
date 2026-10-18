---
api_specs:
- filename: loft-labs-healthz-api-openapi.yml
  format: yaml
  label: Loft Labs Healthz API
  slug: loft-labs-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/loft-labs-healthz-api-openapi.yml
- filename: loft-labs-kubernetes-api-openapi.yml
  format: yaml
  label: Loft Labs Kubernetes API
  slug: loft-labs-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/loft-labs-kubernetes-api-openapi.yml
- filename: loft-labs-loft-labs-api-api-openapi.yml
  format: yaml
  label: Loft Labs Loft Labs API
  slug: loft-labs-loft-labs-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/loft-labs-loft-labs-api-api-openapi.yml
- filename: loft-labs-loft-sh-api-openapi.yml
  format: yaml
  label: Loft Labs Loft Sh API
  slug: loft-labs-loft-sh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/loft-labs-loft-sh-api-openapi.yml
- filename: loft-labs-node-api-openapi.yml
  format: yaml
  label: Loft Labs Node API
  slug: loft-labs-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/openapi/loft-labs-node-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loft.sh
  spf: true
hosts:
- cert_expires: Jan  7 12:43:49 2027 GMT
  host: www.loft.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loft Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loft Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loft Labs
provider_slug: loft-labs
slug: loft-labs-domain-security
source_filename: loft-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.loft.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 12:43:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loft.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loft-labs/refs/heads/main/security/loft-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cloud
- Kubernetes
- Multi-Tenant
- Infrastructure
---
