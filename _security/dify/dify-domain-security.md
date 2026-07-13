---
api_specs:
- filename: dify-openapi.yml
  format: yaml
  label: Dify
  slug: dify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dify.ai
  spf: true
hosts:
- cert_expires: Oct  5 03:00:51 2026 GMT
  host: dify.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:07:38 2026 GMT
  host: docs.dify.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 01:32:24 2026 GMT
  host: api.dify.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dify
provider_slug: dify
slug: dify-domain-security
source_filename: dify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:00:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:07:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.dify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 01:32:24 2026 GMT\n  hsts: null\ndomains:\n- domain: dify.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/security/dify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Backend-As-A-Service
- LLMOps
---
