---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: p0stman.com
  spf: false
hosts:
- cert_expires: Oct 19 15:01:36 2026 GMT
  host: p0stman.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: P0Stman Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for p0stman, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: p0stman
provider_slug: p0stman-com
slug: p0stman-com-domain-security
source_filename: p0stman-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: p0stman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 15:01:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: p0stman.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p0stman-com/refs/heads/main/security/p0stman-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- MCP
- A2A
- Agentic Web
- Voice AI
- AI Automation
- Product Studio
- Software Development
- Consulting
- United Kingdom
---
