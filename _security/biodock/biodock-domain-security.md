---
api_specs:
- filename: biodock-public-api-openapi.yml
  format: yaml
  label: Biodock Public API
  slug: biodock-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biodock/refs/heads/main/openapi/biodock-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biodock.ai
  spf: true
hosts:
- cert_expires: Aug 31 13:19:41 2026 GMT
  host: docs.biodock.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:46:19 2026 GMT
  host: app.biodock.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biodock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biodock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biodock
provider_slug: biodock
slug: biodock-domain-security
source_filename: biodock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.biodock.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:19:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.biodock.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:46:19 2026 GMT\n  hsts: false\ndomains:\n- domain: biodock.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biodock/refs/heads/main/security/biodock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Image Analysis
- Microscopy
- Life Sciences
- Biotechnology
- Computer Vision
- Cell Analysis
- Research
---
