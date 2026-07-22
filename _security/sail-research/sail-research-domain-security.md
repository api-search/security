---
api_specs:
- filename: sail-research-openapi-original.json
  format: json
  label: Sail API
  slug: sail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sail-research/refs/heads/main/openapi/sail-research-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sailresearch.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.sailresearch.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sail Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sail Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sail Research
provider_slug: sail-research
slug: sail-research-domain-security
source_filename: sail-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sailresearch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sailresearch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sail-research/refs/heads/main/security/sail-research-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- Inference
- Agents
- Machine Learning
- Developer Tools
---
