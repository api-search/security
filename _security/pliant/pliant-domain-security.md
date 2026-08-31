---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getpliant.com
  spf: true
hosts:
- cert_expires: Sep 18 14:37:43 2026 GMT
  host: www.getpliant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 10:31:41 2026 GMT
  host: customer-api.getpliant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pliant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pliant, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pliant
provider_slug: pliant
slug: pliant-domain-security
source_filename: pliant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:37:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customer-api.getpliant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:31:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getpliant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pliant/refs/heads/main/security/pliant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Corporate Cards
- Card Issuing
- Spend Management
- Expense Management
- Fintech
- Cards as a Service
- Banking as a Service
- Travel
- Accounting
---
