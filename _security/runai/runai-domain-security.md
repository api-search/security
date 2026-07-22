---
api_specs:
- filename: runai-openapi-original.json
  format: json
  label: NVIDIA Run:ai Control Plane REST API
  slug: nvidia-runai-control-plane-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runai/refs/heads/main/openapi/runai-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nvidia.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: run.ai
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.nvidia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 17:05:16 2026 GMT
  host: run-ai-docs.nvidia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 07:46:04 2026 GMT
  host: app.run.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NVIDIA Run:ai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NVIDIA Run:ai
provider_slug: runai
slug: runai-domain-security
source_filename: runai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: run-ai-docs.nvidia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:05:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.run.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 07:46:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nvidia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: run.ai\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runai/refs/heads/main/security/runai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- GPU
- Machine Learning
- Kubernetes
- Orchestration
- MLOps
- Compute
- Scheduling
- Infrastructure
---
