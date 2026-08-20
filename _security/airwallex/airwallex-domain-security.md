---
api_specs:
- filename: airwallex-authentication-api-openapi.yml
  format: yaml
  label: Airwallex Authentication API
  slug: airwallex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-authentication-api-openapi.yml
- filename: airwallex-balances-api-openapi.yml
  format: yaml
  label: Airwallex Balances API
  slug: airwallex-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-balances-api-openapi.yml
- filename: airwallex-beneficiaries-api-openapi.yml
  format: yaml
  label: Airwallex Beneficiaries API
  slug: airwallex-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-beneficiaries-api-openapi.yml
- filename: airwallex-customers-api-openapi.yml
  format: yaml
  label: Airwallex Customers API
  slug: airwallex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-customers-api-openapi.yml
- filename: airwallex-payment-intents-api-openapi.yml
  format: yaml
  label: Airwallex Payment Intents API
  slug: airwallex-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payment-intents-api-openapi.yml
- filename: airwallex-payouts-api-openapi.yml
  format: yaml
  label: Airwallex Payouts API
  slug: airwallex-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payouts-api-openapi.yml
- filename: airwallex-refunds-api-openapi.yml
  format: yaml
  label: Airwallex Refunds API
  slug: airwallex-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-refunds-api-openapi.yml
- filename: airwallex-transfers-api-openapi.yml
  format: yaml
  label: Airwallex Transfers API
  slug: airwallex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airwallex.com
  spf: true
hosts:
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: www.airwallex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: api.airwallex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: api-demo.airwallex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airwallex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airwallex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airwallex
provider_slug: airwallex
slug: airwallex-domain-security
source_filename: airwallex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airwallex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.airwallex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: null\n- host: api-demo.airwallex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: airwallex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/security/airwallex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cross-Border Payments
- Fintech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
---
