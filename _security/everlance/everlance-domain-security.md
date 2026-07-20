---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: everlance.com
  spf: true
hosts:
- cert_expires: Oct 14 22:17:54 2026 GMT
  host: www.everlance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:40:07 2026 GMT
  host: help.everlance.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.everlance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Everlance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everlance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Everlance
provider_slug: everlance
slug: everlance-domain-security
source_filename: everlance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.everlance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 22:17:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.everlance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.everlance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: everlance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everlance/refs/heads/main/security/everlance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Mileage Tracking
- Expense Management
- Reimbursement
- Fleet Management
- Tax
- Gig Economy
- HR Integration
- Business API
---
