---
api_specs:
- filename: infer-by-flow7-catalog-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Catalog API
  slug: infer-by-flow7-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-catalog-api-openapi.yml
- filename: infer-by-flow7-inference-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Inference API
  slug: infer-by-flow7-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-inference-api-openapi.yml
- filename: infer-by-flow7-status-api-openapi.yml
  format: yaml
  label: Infer by Flow7 Status API
  slug: infer-by-flow7-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/openapi/infer-by-flow7-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flow7.org
  spf: true
hosts:
- cert_expires: Oct 22 16:26:07 2026 GMT
  host: infer.flow7.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infer By Flow7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infer by Flow7, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Infer by Flow7
provider_slug: infer-by-flow7
slug: infer-by-flow7-domain-security
source_filename: infer-by-flow7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infer.flow7.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 16:26:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flow7.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infer-by-flow7/refs/heads/main/security/infer-by-flow7-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI/ML inference
- LLM API gateway
- Responses-compatible API
- Coding-agent tooling
- Developer Tools
- Usage-based billing
- Prepaid billing
- Agent-native
- Agent Skills
- Model routing
---
