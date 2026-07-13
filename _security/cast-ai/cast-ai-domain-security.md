---
api_specs:
- filename: cast-ai-kubernetes-cost-optimization-openapi.yml
  format: yaml
  label: CAST AI Kubernetes Cost Optimization API
  slug: kubernetes-cost-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/openapi/cast-ai-kubernetes-cost-optimization-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cast.ai
  spf: true
hosts:
- cert_expires: Sep  6 09:05:05 2026 GMT
  host: cast.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:22:33 2026 GMT
  host: docs.cast.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 08:22:34 2026 GMT
  host: api.cast.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cast Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CAST AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CAST AI
provider_slug: cast-ai
slug: cast-ai-domain-security
source_filename: cast-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cast.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:05:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.cast.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:22:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cast.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:22:34 2026 GMT\n  hsts: null\ndomains:\n- domain: cast.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cast-ai/refs/heads/main/security/cast-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Autoscaling
- Cloud Infrastructure
- Cost Optimization
- DevOps
- FinOps
- Kubernetes
- Observability
---
