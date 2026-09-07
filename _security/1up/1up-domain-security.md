---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: 1up.ai
  spf: true
hosts:
- cert_expires: Oct  7 14:48:07 2026 GMT
  host: 1up.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 22:43:54 2026 GMT
  host: help.1up.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: mcp.1up.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 1Up Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1up, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: 1up
provider_slug: 1up
slug: 1up-domain-security
source_filename: 1up-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1up.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.1up.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 22:43:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: mcp.1up.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: 1up.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1up/refs/heads/main/security/1up-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Knowledge Management
- RFP Automation
- Security Questionnaires
- Model Context Protocol
- Agents
- SaaS
- Revenue Operations
---
