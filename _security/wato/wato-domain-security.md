---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: watolabs.com
  spf: false
hosts:
- cert_expires: Sep 30 07:17:57 2026 GMT
  host: docs.watolabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 07:17:57 2026 GMT
  host: mesh.watolabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wato, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Wato
provider_slug: wato
slug: wato-domain-security
source_filename: wato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.watolabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 07:17:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mesh.watolabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 07:17:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: watolabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wato/refs/heads/main/security/wato-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Agent Governance
- Team Memory
- Connectors
- Agent Skills
- Automation
- Developer Tools
- Y Combinator
---
