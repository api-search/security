---
api_specs:
- filename: tenyks-openapi.json
  format: json
  label: Tenyks API
  slug: tenyks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenyks/refs/heads/main/openapi/tenyks-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tenyks.ai
  spf: true
hosts:
- cert_expires: Oct  7 05:06:30 2026 GMT
  host: docs.tenyks.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: dashboard.tenyks.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenyks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenyks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tenyks
provider_slug: tenyks
slug: tenyks-domain-security
source_filename: tenyks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.tenyks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 05:06:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.tenyks.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tenyks.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenyks/refs/heads/main/security/tenyks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computer Vision
- Machine Learning
- MLOps
- Data Quality
- Model Validation
- Visual Intelligence
- Video Analytics
- Artificial Intelligence
- Developer Tools
---
