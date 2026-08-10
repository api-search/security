---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meshpayments.com
  spf: true
hosts:
- cert_expires: Oct  2 11:09:24 2026 GMT
  host: meshpayments.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: developers.meshpayments.com
  hsts: false
  https: true
  note: served by CloudFront behind HTTP Basic authentication (401 with WWW-Authenticate Basic); no Strict-Transport-Security header observed on the 401 response
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.meshpayments.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Strict-Transport-Security max-age=31536000 includeSubDomains observed on the 401 challenge response
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mesh Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mesh Payments, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mesh Payments
provider_slug: mesh-payments
slug: mesh-payments-domain-security
source_filename: mesh-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meshpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:09:24 2026 GMT\n  hsts: false\n- host: developers.meshpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n  note: served by CloudFront behind HTTP Basic authentication (401 with WWW-Authenticate\n    Basic); no Strict-Transport-Security header observed on the 401 response\n- host: api.meshpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Strict-Transport-Security max-age=31536000 includeSubDomains observed on the\n    401 challenge response\ndomains:\n- domain: meshpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-payments/refs/heads/main/security/mesh-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Spend Management
- Expense Management
- Corporate Cards
- Travel
- Accounts Payable
- Fintech
- Card Issuing
- Accounting Automation
---
