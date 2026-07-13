---
api_specs:
- filename: opencost-openapi.yml
  format: yaml
  label: OpenCost API
  slug: opencost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencost/refs/heads/main/openapi/opencost-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencost.io
  spf: false
hosts:
- cert_expires: Sep 10 03:36:04 2026 GMT
  host: opencost.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 03:36:04 2026 GMT
  host: www.opencost.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCost, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenCost
provider_slug: opencost
slug: opencost-domain-security
source_filename: opencost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:36:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.opencost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:36:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opencost.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencost/refs/heads/main/security/opencost-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Cost Management
- CNCF
- FinOps
- Kubernetes
- Observability
---
