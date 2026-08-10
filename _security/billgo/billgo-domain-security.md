---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: billgo.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: billgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 13:23:31 2026 GMT
  host: docs.billgo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: exchange.billgo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Billgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BillGO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BillGO
provider_slug: billgo
slug: billgo-domain-security
source_filename: billgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.billgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 13:23:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: exchange.billgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: billgo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billgo/refs/heads/main/security/billgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Bill Pay
- Financial Services
- Banking
- ACH
- Virtual Cards
- Fintech
- GraphQL
---
