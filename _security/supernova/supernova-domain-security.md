---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: supernova.io
  spf: true
hosts:
- cert_expires: Sep 21 03:13:53 2026 GMT
  host: www.supernova.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Supernova Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supernova, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Supernova
provider_slug: supernova
slug: supernova-domain-security
source_filename: supernova-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.supernova.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:13:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: supernova.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supernova/refs/heads/main/security/supernova-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Design Tech
- Design Systems
- Design Tokens
- Documentation
- Code Automation
- Developer Experience
- AI Agents
- MCP
---
