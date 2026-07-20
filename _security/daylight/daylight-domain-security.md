---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daylight.ai
  spf: true
hosts:
- cert_expires: Oct  9 02:56:36 2026 GMT
  host: daylight.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 16:14:37 2026 GMT
  host: docs.daylight.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.daylight.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daylight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daylight, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daylight
provider_slug: daylight
slug: daylight-domain-security
source_filename: daylight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daylight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:56:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.daylight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 16:14:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.daylight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: daylight.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daylight/refs/heads/main/security/daylight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- MDR
- Threat Detection
- Incident Response
- Agentic AI
- SOC
- MCP
---
