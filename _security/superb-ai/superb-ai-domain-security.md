---
api_specs:
- filename: superb-ai-mlops-platform-openapi.json
  format: json
  label: Superb AI MLOps Platform API
  slug: superb-ai-mlops-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superb-ai/refs/heads/main/openapi/superb-ai-mlops-platform-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: superb-ai.com
  spf: true
hosts:
- cert_expires: Oct 21 19:48:11 2026 GMT
  host: superb-ai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: docs.bdai.superb-ai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.bdai.superb-ai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superb Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superb AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Superb AI
provider_slug: superb-ai
slug: superb-ai-domain-security
source_filename: superb-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superb-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 19:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bdai.superb-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: api.bdai.superb-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: superb-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superb-ai/refs/heads/main/security/superb-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Machine Learning
- Computer Vision
- Data Labeling
- Annotation
- MLOps
- Training Data
- Model Training
- Inference
- Datasets
---
