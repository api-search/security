---
api_specs:
- filename: quantcdn-openapi.yml
  format: yaml
  label: QuantCDN API
  slug: quantcdn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quantcdn/refs/heads/main/openapi/quantcdn-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quantcdn.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: quantgov.cloud
  spf: false
hosts:
- cert_expires: Sep 23 10:18:30 2026 GMT
  host: www.quantcdn.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 10:18:30 2026 GMT
  host: dashboard.quantcdn.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: dash.quantgov.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantcdn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QuantCDN, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QuantCDN
provider_slug: quantcdn
slug: quantcdn-domain-security
source_filename: quantcdn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quantcdn.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:18:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.quantcdn.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:18:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dash.quantgov.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quantcdn.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: quantgov.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantcdn/refs/heads/main/security/quantcdn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDN
- Edge
- Static Hosting
- Jamstack
- DNS
- WAF
- Edge Computing
- Key-Value Storage
- AI Inference
---
