---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blitzy.com
  spf: true
hosts:
- cert_expires: Sep 19 02:57:27 2026 GMT
  host: blitzy.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blitzy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blitzy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blitzy
provider_slug: blitzy
slug: blitzy-domain-security
source_filename: blitzy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blitzy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: blitzy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blitzy/refs/heads/main/security/blitzy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Artificial Intelligence
- Software Development
- Code Generation
- Autonomous Agents
- Legacy Modernization
- Developer Tools
- Enterprise
---
