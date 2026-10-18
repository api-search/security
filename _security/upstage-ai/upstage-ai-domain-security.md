---
api_specs:
- filename: upstage-ai-system-one-api-openapi.yml
  format: yaml
  label: Upstage System One API
  slug: upstage-ai-system-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upstage-ai/refs/heads/main/openapi/upstage-ai-system-one-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upstage.ai
  spf: true
hosts:
- cert_expires: Nov 21 20:29:33 2026 GMT
  host: upstage.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: console.upstage.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 27 23:59:59 2027 GMT
  host: api.upstage.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Upstage Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upstage, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upstage
provider_slug: upstage-ai
slug: upstage-ai-domain-security
source_filename: upstage-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upstage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 20:29:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.upstage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upstage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: upstage.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstage-ai/refs/heads/main/security/upstage-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Document AI
- OCR
- Decision Support
- Structured Outputs
- Embeddings
---
