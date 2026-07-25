---
api_specs:
- filename: navan-bookings-api-openapi.yml
  format: yaml
  label: Navan Bookings API
  slug: navan-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-bookings-api-openapi.yml
- filename: navan-custom-fields-api-openapi.yml
  format: yaml
  label: Navan Custom Fields API
  slug: navan-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-custom-fields-api-openapi.yml
- filename: navan-fees-and-adjustments-api-openapi.yml
  format: yaml
  label: Navan Fees and Adjustments API
  slug: navan-fees-and-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-fees-and-adjustments-api-openapi.yml
- filename: navan-receipts-api-openapi.yml
  format: yaml
  label: Navan Receipts API
  slug: navan-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-receipts-api-openapi.yml
- filename: navan-transactions-api-openapi.yml
  format: yaml
  label: Navan Transactions API
  slug: navan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-transactions-api-openapi.yml
- filename: navan-users-api-openapi.yml
  format: yaml
  label: Navan Users API
  slug: navan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-users-api-openapi.yml
- filename: navan-webhooks-api-openapi.yml
  format: yaml
  label: Navan Webhooks API
  slug: navan-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/openapi/navan-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "www.digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
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
- cert_expires: Aug 20 14:41:22 2026 GMT
  host: developer.navan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 14:41:22 2026 GMT
  host: api.navan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Navan
provider_slug: navan
slug: navan-domain-security
source_filename: navan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: navan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.navan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.navan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 14:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: navan.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/security/navan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Corporate Travel
- Expense Management
- Corporate Cards
- Spend Management
- T&E
- Fintech
- Business Travel
---
