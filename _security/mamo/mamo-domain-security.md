---
api_specs:
- filename: mamo-openapi.yml
  format: yaml
  label: Mamo Business API
  slug: mamo-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/openapi/mamo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:caa-violations@mamopay.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mamopay.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 10 12:51:52 2026 GMT
  host: mamopay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: mamopay.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:01:17 2026 GMT
  host: business.mamopay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mamo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mamo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mamo
provider_slug: mamo
slug: mamo-domain-security
source_filename: mamo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mamopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:51:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mamopay.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: business.mamopay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:01:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mamopay.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:caa-violations@mamopay.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mamo/refs/heads/main/security/mamo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Payment Links
- Subscriptions
- Corporate Cards
- Payouts
- Expense Management
- UAE
- Middle East
---
