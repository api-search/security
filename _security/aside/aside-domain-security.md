---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aside.com
  spf: true
hosts:
- cert_expires: Aug 20 09:13:44 2026 GMT
  host: aside.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aside, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aside
provider_slug: aside
slug: aside-domain-security
source_filename: aside-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aside.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 09:13:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aside.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aside/refs/heads/main/security/aside-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Browser
- Browser Agent
- Automation
- Model Context Protocol
- MCP
- CLI
- Password Manager
- Agentic
- Web Automation
- Developer Tools
- Y Combinator
---
