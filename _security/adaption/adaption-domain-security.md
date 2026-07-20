---
api_specs:
- filename: adaption-adaptive-data-api-openapi.yml
  format: yaml
  label: Adaptive Data API
  slug: adaptive-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaption/refs/heads/main/openapi/adaption-adaptive-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adaptionlabs.ai
  spf: true
hosts:
- cert_expires: Sep  3 16:46:31 2026 GMT
  host: docs.adaptionlabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.prod.adaptionlabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Adaption Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaption, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adaption
provider_slug: adaption
slug: adaption-domain-security
source_filename: adaption-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.adaptionlabs.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 16:46:31 2026 GMT\n  hsts: false\n- host: api.prod.adaptionlabs.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adaptionlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaption/refs/heads/main/security/adaption-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Machine Learning
- Training Data
- Datasets
- Data Augmentation
- LLM
- Model Training
- Developer Tools
---
