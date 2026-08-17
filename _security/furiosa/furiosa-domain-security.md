---
api_specs:
- filename: furiosa-predict-v2.yaml
  format: yaml
  label: Furiosa Model Server - Predict API (KServe v2)
  slug: furiosa-server-predict-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/furiosa/refs/heads/main/openapi/furiosa-predict-v2.yaml
- filename: furiosa-model-repository-v2.yaml
  format: yaml
  label: Furiosa Model Server - Model Repository API
  slug: furiosa-model-repository-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/furiosa/refs/heads/main/openapi/furiosa-model-repository-v2.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: furiosa.ai
  spf: false
hosts:
- cert_expires: Sep 23 01:42:15 2026 GMT
  host: furiosa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:42:48 2026 GMT
  host: developer.furiosa.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Furiosa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FuriosaAI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: FuriosaAI
provider_slug: furiosa
slug: furiosa-domain-security
source_filename: furiosa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: furiosa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:42:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.furiosa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:42:48 2026 GMT\n  hsts: false\ndomains:\n- domain: furiosa.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/furiosa/refs/heads/main/security/furiosa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Machine Learning
- Inference
- Semiconductors
- NPU
- Hardware
- LLM
- Model Serving
- Kubernetes
- Developer Tools
- Compute
- Infrastructure
---
