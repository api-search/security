---
api_specs:
- filename: humanloop-openapi.yml
  format: yaml
  label: Humanloop LLM Platform API
  slug: llm-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanloop/refs/heads/main/openapi/humanloop-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humanloop.com
  spf: true
hosts:
- cert_expires: Aug 18 13:30:43 2026 GMT
  host: humanloop.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.humanloop.com
  https: false
kind: domain-security
layout: security
method: probed
name: Humanloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humanloop, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Humanloop
provider_slug: humanloop
slug: humanloop-domain-security
source_filename: humanloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanloop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:30:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.humanloop.com\n  https: false\ndomains:\n- domain: humanloop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanloop/refs/heads/main/security/humanloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM Platform
- Prompt Management
- Evaluations
- LLM Ops
- Observability
- Datasets
- Prompts
- Tools
- Logs
- Multi-Provider
- Sunsetting
- Acquired
---
