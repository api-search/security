---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: macro.com
  spf: true
hosts:
- cert_expires: Sep 15 07:16:12 2026 GMT
  host: docs.macro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: mcp-server.macro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Macro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macro, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Macro
provider_slug: macro
slug: macro-domain-security
source_filename: macro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.macro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:16:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mcp-server.macro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: macro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macro/refs/heads/main/security/macro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Email
- Collaboration
- Workspace
- CRM
- Tasks
- AI Agents
- MCP
- Open Source
---
