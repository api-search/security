---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reevo.ai
  spf: true
hosts:
- cert_expires: Nov  1 23:17:44 2026 GMT
  host: www.reevo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 01:39:46 2026 GMT
  host: help.reevo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.reevo.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 00:19:54 2026 GMT
  host: mcp.reevo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 09:34:06 2026 GMT
  host: login.reevo.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: app.reevo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reevo, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reevo
provider_slug: reevo
slug: reevo-domain-security
source_filename: reevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:17:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 01:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\n- host: mcp.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:19:54 2026 GMT\n  hsts: false\n- host: login.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:34:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: reevo.ai\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reevo/refs/heads/main/security/reevo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Sales
- CRM
- Revenue Operations
- Sales Automation
- Lead Generation
- Agents
- MCP
- Sales Engagement
---
