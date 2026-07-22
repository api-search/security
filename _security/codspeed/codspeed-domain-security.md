---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codspeed.io
  spf: true
hosts:
- cert_expires: Aug 22 10:41:59 2026 GMT
  host: codspeed.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codspeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodSpeed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CodSpeed
provider_slug: codspeed
slug: codspeed-domain-security
source_filename: codspeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codspeed.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:41:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: codspeed.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codspeed/refs/heads/main/security/codspeed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Performance
- Benchmarking
- Continuous Integration
- Developer Tools
- Observability
- Testing
- DevOps
- AI
- MCP
---
