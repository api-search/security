---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getzipline.com
  spf: true
hosts:
- cert_expires: Nov 14 20:26:22 2026 GMT
  host: getzipline.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retail Zipline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Retail Zipline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Retail Zipline
provider_slug: retail-zipline
slug: retail-zipline-domain-security
source_filename: retail-zipline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getzipline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 20:26:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getzipline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retail-zipline/refs/heads/main/security/retail-zipline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Retail Operations
- Task Management
- Employee Communications
- Store Operations
- Workforce
- Knowledge Base
- Software-as-a-Service
- MCP
- Company
---
