---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hakuto-0209.com
  spf: false
hosts:
- cert_expires: Oct 26 23:35:53 2026 GMT
  host: hakuto-0209.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hakuto 0209 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HaneruTo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HaneruTo
provider_slug: hakuto-0209-com
slug: hakuto-0209-com-domain-security
source_filename: hakuto-0209-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hakuto-0209.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:35:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hakuto-0209.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakuto-0209-com/refs/heads/main/security/hakuto-0209-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agents
- MCP
- A2A
- Code Review
- Static Analysis
- Developer Tools
- Compliance
- Web Development
- Japan
- Agent-Native
---
