---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jigso.io
  spf: true
hosts:
- cert_expires: Sep  9 22:02:17 2026 GMT
  host: www.jigso.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.jigso.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jigso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jigso, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Jigso
provider_slug: jigso
slug: jigso-domain-security
source_filename: jigso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jigso.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.jigso.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: jigso.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jigso/refs/heads/main/security/jigso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Enterprise
- Business Intelligence
- Revenue Operations
- Model Context Protocol
- Agents
- Data Integration
- Customer Success
- Sales
---
