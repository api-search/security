---
api_specs:
- filename: exa-openapi.yml
  format: yaml
  label: Exa Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exa/refs/heads/main/openapi/exa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exa.ai
  spf: true
hosts:
- cert_expires: Sep 13 19:42:12 2026 GMT
  host: exa.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 04:45:50 2026 GMT
  host: api.exa.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exa, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Exa
provider_slug: exa
slug: exa-domain-security
source_filename: exa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:42:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.exa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:45:50 2026 GMT\n  hsts: null\ndomains:\n- domain: exa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exa/refs/heads/main/security/exa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Neural Search
- AI Agents
- LLMs
- Web Index
- Retrieval
- Answer
- Contents
- Find Similar
- Research
- SOC 2
- MCP
---
