---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: perk.com
  spf: true
hosts:
- cert_expires: Sep 28 19:54:20 2026 GMT
  host: developers.perk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.perk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: app.perk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Perk
provider_slug: perk
slug: perk-domain-security
source_filename: perk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.perk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:54:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.perk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: app.perk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: perk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/security/perk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Corporate Travel
- Expense Management
- Spend Management
- Travel
- Invoices
- Fintech
- SaaS
---
