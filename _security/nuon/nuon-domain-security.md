---
api_specs:
- filename: nuon-oapi-v3-openapi.json
  format: json
  label: Nuon Control Plane API
  slug: nuon-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-oapi-v3-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nuon.co
  spf: true
hosts:
- cert_expires: Oct 13 10:43:03 2026 GMT
  host: nuon.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 19:30:28 2026 GMT
  host: docs.nuon.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.nuon.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nuon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nuon
provider_slug: nuon
slug: nuon-domain-security
source_filename: nuon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuon.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nuon.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 19:30:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nuon.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nuon.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/security/nuon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- BYOC
- Deployment
- Continuous Delivery
- DevOps
- Infrastructure
- Cloud
- Multi-Cloud
- Kubernetes
- Terraform
- Platform Engineering
---
