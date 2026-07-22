---
api_specs:
- filename: sail-openapi-original.json
  format: json
  label: Sail API
  slug: sail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/openapi/sail-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sailresearch.com
  spf: true
hosts:
- cert_expires: Aug 25 02:17:20 2026 GMT
  host: www.sailresearch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.sailresearch.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sail, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sail
provider_slug: sail
slug: sail-domain-security
source_filename: sail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sailresearch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 02:17:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sailresearch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sailresearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sail/refs/heads/main/security/sail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Machine Learning
- LLM
- Inference
- Agents
- Open Source Models
- Infrastructure
- Developer Tools
---
