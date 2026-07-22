---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: silmaril.dev
  spf: false
hosts:
- cert_expires: Sep 18 10:25:32 2026 GMT
  host: silmaril.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:07:00 2026 GMT
  host: firewall-mcp.silmaril.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silmaril Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silmaril, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Silmaril
provider_slug: silmaril
slug: silmaril-domain-security
source_filename: silmaril-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silmaril.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:25:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: firewall-mcp.silmaril.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:07:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: silmaril.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silmaril/refs/heads/main/security/silmaril-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI Security
- AI Firewall
- Prompt Injection
- Agent Security
- Runtime Security
- Guardrails
- MCP
- LLM Security
- Developer Tools
---
