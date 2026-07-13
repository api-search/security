---
api_specs:
- filename: baseten-llm-openapi.json
  format: json
  label: Baseten LLM Inference API
  slug: llm-inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baseten/refs/heads/main/openapi/baseten-llm-openapi.json
- filename: baseten-messages-openapi.json
  format: json
  label: Baseten Anthropic-Compatible Messages API
  slug: messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/baseten/refs/heads/main/openapi/baseten-messages-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: baseten.co
  spf: true
hosts:
- cert_expires: Sep 11 13:15:58 2026 GMT
  host: www.baseten.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 13:34:14 2026 GMT
  host: docs.baseten.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:06:53 2026 GMT
  host: inference.baseten.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baseten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baseten, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Baseten
provider_slug: baseten
slug: baseten-domain-security
source_filename: baseten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baseten.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.baseten.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 13:34:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: inference.baseten.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:06:53 2026 GMT\n  hsts: null\ndomains:\n- domain: baseten.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baseten/refs/heads/main/security/baseten-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- ML
- Inference
- Deployment
- MLOps
- OpenAI Compatible
- Anthropic Compatible
- Truss
---
