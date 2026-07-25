---
api_specs:
- filename: creem-checkouts-api-openapi.yml
  format: yaml
  label: Creem Checkouts API
  slug: creem-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-checkouts-api-openapi.yml
- filename: creem-customers-api-openapi.yml
  format: yaml
  label: Creem Customers API
  slug: creem-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-customers-api-openapi.yml
- filename: creem-discounts-api-openapi.yml
  format: yaml
  label: Creem Discounts API
  slug: creem-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-discounts-api-openapi.yml
- filename: creem-licenses-api-openapi.yml
  format: yaml
  label: Creem Licenses API
  slug: creem-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-licenses-api-openapi.yml
- filename: creem-products-api-openapi.yml
  format: yaml
  label: Creem Products API
  slug: creem-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-products-api-openapi.yml
- filename: creem-subscriptions-api-openapi.yml
  format: yaml
  label: Creem Subscriptions API
  slug: creem-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-subscriptions-api-openapi.yml
- filename: creem-transactions-api-openapi.yml
  format: yaml
  label: Creem Transactions API
  slug: creem-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/openapi/creem-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creem.io
  spf: true
hosts:
- cert_expires: Oct  1 05:25:16 2026 GMT
  host: www.creem.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 08:54:21 2026 GMT
  host: docs.creem.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:22:56 2026 GMT
  host: api.creem.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creem, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Creem
provider_slug: creem
slug: creem-domain-security
source_filename: creem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:25:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.creem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:54:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.creem.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:22:56 2026 GMT\n  hsts: false\ndomains:\n- domain: creem.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creem/refs/heads/main/security/creem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Merchant of Record
- Subscriptions
- SaaS
- Billing
---
