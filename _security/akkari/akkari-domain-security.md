---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: akkari.io
  spf: true
hosts:
- cert_expires: Aug 24 08:15:42 2026 GMT
  host: akkari.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akkari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akkari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Akkari
provider_slug: akkari
slug: akkari-domain-security
source_filename: akkari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akkari.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:15:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: akkari.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akkari/refs/heads/main/security/akkari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Operations
- Customer Success
- Artificial Intelligence
- Automation
- Workflow Automation
- SaaS
- Y Combinator
- AI Agents
---
