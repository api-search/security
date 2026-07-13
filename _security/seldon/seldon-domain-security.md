---
api_specs:
- filename: engine.oas3.json
  format: json
  label: Seldon Inference API
  slug: seldon-inference-api
  spec_type: OpenAPI
  url: https://github.com/SeldonIO/seldon-core/blob/master/openapi/engine.oas3.json
- filename: seldon-enterprise-platform-api-openapi.yml
  format: yaml
  label: Seldon Enterprise Platform REST API
  slug: seldon-enterprise-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/openapi/seldon-enterprise-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: seldon.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: seldon.ai
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.seldon.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 05:08:52 2026 GMT
  host: docs.seldon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: deploy.seldon.io
  https: false
kind: domain-security
layout: security
method: probed
name: Seldon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seldon, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Seldon
provider_slug: seldon
slug: seldon-domain-security
source_filename: seldon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seldon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\n- host: docs.seldon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 05:08:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: deploy.seldon.io\n  https: false\ndomains:\n- domain: seldon.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: seldon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seldon/refs/heads/main/security/seldon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- MLOps
- Machine Learning
- Model Serving
- Inference
- Kubernetes
- AI Operations
- Drift Detection
- Explainability
- Canary Deployment
- A/B Testing
- LLMOps
---
