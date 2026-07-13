---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: open.money
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zwitch.io
  spf: true
hosts:
- cert_expires: Dec  8 05:18:17 2026 GMT
  host: open.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 02:31:34 2026 GMT
  host: www.zwitch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 00:04:25 2026 GMT
  host: developers.zwitch.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open (open.money), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open (open.money)
provider_slug: open-financial
slug: open-financial-domain-security
source_filename: open-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 05:18:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.zwitch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.zwitch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:04:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: open.money\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zwitch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-financial/refs/heads/main/security/open-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Banking
- Neobank
- SMB
- Embedded Finance
- Banking as a Service
- Payments
- Payouts
- UPI
- Accounting
- Payroll
- Expense Management
- India
- Fintech
---
