---
api_specs:
- filename: plaid-plaid-api-openapi.yml
  format: yaml
  label: Plaid Plaid API
  slug: plaid-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-plaid-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plaid.com
  spf: true
hosts:
- host: developer.plaid.com
  https: false
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: plaid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: production.plaid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Plaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plaid, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Plaid
provider_slug: plaid
slug: plaid-domain-security
source_filename: plaid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.plaid.com\n  https: false\n- host: plaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.plaid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: plaid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/security/plaid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Fintech
- Open Banking
- Bank Accounts
- Data Aggregation
- Payments
- United States
---
