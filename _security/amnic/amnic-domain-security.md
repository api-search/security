---
api_specs:
- filename: amnic-openapi.yml
  format: yaml
  label: Amnic Cloud Cost Observability API
  slug: amnic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/openapi/amnic-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amnic.com
  spf: true
hosts:
- cert_expires: Sep 20 15:02:14 2026 GMT
  host: amnic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:07:20 2026 GMT
  host: api.amnic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amnic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amnic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amnic
provider_slug: amnic
slug: amnic-domain-security
source_filename: amnic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amnic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:02:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.amnic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:07:20 2026 GMT\n  hsts: null\ndomains:\n- domain: amnic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/security/amnic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Cost Observability
- FinOps
- Cloud Cost Management
- Cost Optimization
- Kubernetes
- Azure
- Google Cloud
---
