---
api_specs:
- filename: unisson-openapi-original.json
  format: json
  label: Unisson Platform API
  slug: unisson-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/openapi/unisson-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unisson.ai
  spf: true
hosts:
- cert_expires: Oct 12 15:43:29 2026 GMT
  host: www.unisson.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.unisson.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unisson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unisson, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unisson
provider_slug: unisson
slug: unisson-domain-security
source_filename: unisson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unisson.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:43:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unisson.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unisson.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/security/unisson-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Success
- B2B Software
- Implementation
- Automation
- Agents
---
