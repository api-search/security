---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: navan.com
  spf: true
hosts:
- cert_expires: Aug 20 14:41:22 2026 GMT
  host: navan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navan Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Navan
provider_slug: navan-com
slug: navan-com-domain-security
source_filename: navan-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: navan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: navan.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navan-com/refs/heads/main/security/navan-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corporate Travel
- Travel Management
- Expense Management
- Corporate Cards
- Payments
- Spend Management
- Booking
- SCIM
- User Management
- FinTech
- SaaS
- TripActions
---
