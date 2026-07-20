---
api_specs:
- filename: digits-openapi-original.json
  format: json
  label: Digits Connect API
  slug: digits-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits/refs/heads/main/openapi/digits-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: digits.com
  spf: true
hosts:
- cert_expires: Sep 23 01:42:47 2026 GMT
  host: digits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 17:15:38 2026 GMT
  host: developer.digits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:55:24 2026 GMT
  host: connect.digits.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digits, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Digits
provider_slug: digits
slug: digits-domain-security
source_filename: digits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 01:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.digits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.digits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:55:24 2026 GMT\n  hsts: null\ndomains:\n- domain: digits.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits/refs/heads/main/security/digits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Bookkeeping
- Financial Reporting
- General Ledger
- AI
- Fintech
- Accountants
- Bill Pay
- Invoicing
---
