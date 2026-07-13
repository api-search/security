---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: billdesk.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: billdesk.io
  spf: false
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.billdesk.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 08:30:53 2026 GMT
  host: docs.billdesk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.billdesk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Billdesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BillDesk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BillDesk
provider_slug: billdesk
slug: billdesk-domain-security
source_filename: billdesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.billdesk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: docs.billdesk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:30:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.billdesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: billdesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: billdesk.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billdesk/refs/heads/main/security/billdesk-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Payments
- India
- Payment Gateway
- UPI
- Recurring Payments
- Mandates
- Net Banking
- Bill Payments
- Fintech
---
