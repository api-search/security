---
api_specs:
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Evaluations API
  slug: uptrain-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Log and Evaluate API
  slug: uptrain-log-and-evaluate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Root Cause Analysis API
  slug: uptrain-root-cause-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
- filename: uptrain-openapi.yml
  format: yaml
  label: UpTrain Runs and Datasets API
  slug: uptrain-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/openapi/uptrain-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uptrain.ai
  spf: true
hosts:
- cert_expires: Sep 24 14:21:17 2026 GMT
  host: uptrain.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 07:22:30 2026 GMT
  host: docs.uptrain.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: demo.uptrain.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Uptrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UpTrain, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: UpTrain
provider_slug: uptrain
slug: uptrain-domain-security
source_filename: uptrain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptrain.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:21:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.uptrain.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 07:22:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.uptrain.ai\n  https: false\ndomains:\n- domain: uptrain.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptrain/refs/heads/main/security/uptrain-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- LLM
- Evaluation
- LLM Evaluation
- Observability
- Open Source
---
