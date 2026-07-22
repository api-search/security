---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emburse.com
  spf: true
hosts:
- cert_expires: Sep 22 22:18:59 2026 GMT
  host: www.emburse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chrome River Emburse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chrome River (Emburse), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chrome River (Emburse)
provider_slug: chrome-river-emburse
slug: chrome-river-emburse-domain-security
source_filename: chrome-river-emburse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emburse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:18:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: emburse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chrome-river-emburse/refs/heads/main/security/chrome-river-emburse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Expense Management
- Travel And Expense
- Invoice Management
- Corporate Cards
- Spend Management
- Fintech
- Enterprise Software
---
