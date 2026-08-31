---
api_specs:
- filename: sumup-checkouts-api-openapi.yml
  format: yaml
  label: SumUp Checkouts API
  slug: sumup-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-checkouts-api-openapi.yml
- filename: sumup-customers-api-openapi.yml
  format: yaml
  label: SumUp Customers API
  slug: sumup-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-customers-api-openapi.yml
- filename: sumup-members-api-openapi.yml
  format: yaml
  label: SumUp Members API
  slug: sumup-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-members-api-openapi.yml
- filename: sumup-memberships-api-openapi.yml
  format: yaml
  label: SumUp Memberships API
  slug: sumup-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-memberships-api-openapi.yml
- filename: sumup-merchants-api-openapi.yml
  format: yaml
  label: SumUp Merchants API
  slug: sumup-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-merchants-api-openapi.yml
- filename: sumup-payouts-api-openapi.yml
  format: yaml
  label: SumUp Payouts API
  slug: sumup-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-payouts-api-openapi.yml
- filename: sumup-readers-api-openapi.yml
  format: yaml
  label: SumUp Readers API
  slug: sumup-readers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-readers-api-openapi.yml
- filename: sumup-receipts-api-openapi.yml
  format: yaml
  label: SumUp Receipts API
  slug: sumup-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-receipts-api-openapi.yml
- filename: sumup-roles-api-openapi.yml
  format: yaml
  label: SumUp Roles API
  slug: sumup-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-roles-api-openapi.yml
- filename: sumup-transactions-api-openapi.yml
  format: yaml
  label: SumUp Transactions API
  slug: sumup-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/openapi/sumup-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sumup.com
  spf: true
hosts:
- cert_expires: Sep 26 17:57:09 2026 GMT
  host: sumup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 15:12:21 2026 GMT
  host: developer.sumup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 12:32:06 2026 GMT
  host: api.sumup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sumup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SumUp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SumUp
provider_slug: sumup
slug: sumup-domain-security
source_filename: sumup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:57:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sumup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:12:21 2026 GMT\n  hsts: false\n- host: api.sumup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:32:06 2026 GMT\n  hsts: null\ndomains:\n- domain: sumup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/security/sumup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- POS
- Point-of-Sale
- Card Readers
- Checkout
- Fintech
- Mobile Payments
- Online Payments
---
