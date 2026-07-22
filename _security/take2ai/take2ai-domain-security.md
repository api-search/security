---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: take2.ai
  spf: true
hosts:
- cert_expires: Oct  5 17:42:13 2026 GMT
  host: take2.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Take2Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Take2.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Take2.ai
provider_slug: take2ai
slug: take2ai-domain-security
source_filename: take2ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: take2.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 17:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: take2.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/take2ai/refs/heads/main/security/take2ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Recruiting
- Artificial Intelligence
- AI Agents
- Human Resources
- Talent Acquisition
- Hiring
---
