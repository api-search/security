---
api_specs:
- filename: llmabacus-openapi-generated.yml
  format: yaml
  label: LLM Abacus API
  slug: llmabacus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmabacus/refs/heads/main/openapi/_ae-authored/llmabacus-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llmabacus.com
  spf: true
hosts:
- cert_expires: Dec 21 14:15:16 2026 GMT
  host: llmabacus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmabacus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLM Abacus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LLM Abacus
provider_slug: llmabacus
slug: llmabacus-domain-security
source_filename: llmabacus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmabacus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 14:15:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: llmabacus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmabacus/refs/heads/main/security/llmabacus-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- LLM
- API
- Pricing
- Comparison
---
