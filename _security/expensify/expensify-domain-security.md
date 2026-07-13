---
api_specs:
- filename: expensify-openapi.yml
  format: yaml
  label: Expensify Integration Server API
  slug: integration-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expensify/refs/heads/main/openapi/expensify-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "www.digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expensify.com
  spf: true
hosts:
- cert_expires: Aug 31 15:48:42 2026 GMT
  host: www.expensify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 13:38:08 2026 GMT
  host: integrations.expensify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expensify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expensify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Expensify
provider_slug: expensify
slug: expensify-domain-security
source_filename: expensify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expensify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:48:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrations.expensify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 13:38:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: expensify.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"www.digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expensify/refs/heads/main/security/expensify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Expense Management
- Expense Reporting
- Receipt Scanning
- Corporate Cards
- Bill Pay
- Reimbursement
- Accounting Integration
---
