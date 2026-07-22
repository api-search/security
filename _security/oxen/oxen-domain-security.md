---
api_specs:
- filename: oxen-hub-api-openapi-original.json
  format: json
  label: Oxen Hub AI & Fine-Tuning API
  slug: oxen-hub-ai-fine-tuning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-hub-api-openapi-original.json
- filename: oxen-server-openapi-original.json
  format: json
  label: Oxen Data Version Control Server API
  slug: oxen-data-version-control-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-server-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oxen.ai
  spf: true
hosts:
- cert_expires: Oct 14 14:01:16 2026 GMT
  host: www.oxen.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:53:34 2026 GMT
  host: docs.oxen.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: hub.oxen.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oxen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oxen, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oxen
provider_slug: oxen
slug: oxen-domain-security
source_filename: oxen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oxen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:01:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.oxen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:53:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hub.oxen.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oxen.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/security/oxen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Version Control
- Machine Learning
- Artificial Intelligence
- Fine-Tuning
- Inference
- Datasets
- MLOps
- Large Language Models
- Model Deployment
- Developer Tools
- Version Control
---
