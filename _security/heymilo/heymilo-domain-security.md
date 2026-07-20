---
api_specs:
- filename: heymilo-openapi-original.json
  format: json
  label: HeyMilo Public API
  slug: heymilo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/openapi/heymilo-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heymilo.ai
  spf: true
hosts:
- cert_expires: Oct 13 09:46:12 2026 GMT
  host: www.heymilo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 15:40:44 2026 GMT
  host: docs.heymilo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:29:51 2026 GMT
  host: api.heymilo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heymilo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HeyMilo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HeyMilo
provider_slug: heymilo
slug: heymilo-domain-security
source_filename: heymilo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heymilo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 09:46:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.heymilo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:40:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.heymilo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:29:51 2026 GMT\n  hsts: null\ndomains:\n- domain: heymilo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heymilo/refs/heads/main/security/heymilo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Hiring
- Human Resources
- HR Tech
- Artificial Intelligence
- AI Agents
- Interviewing
- Candidate Screening
- Voice AI
- Webhooks
- ATS Integration
---
