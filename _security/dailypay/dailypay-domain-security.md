---
api_specs:
- filename: dailypay-accounts-api-openapi.yml
  format: yaml
  label: DailyPay Accounts API
  slug: dailypay-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-accounts-api-openapi.yml
- filename: dailypay-card-tokenization-api-openapi.yml
  format: yaml
  label: DailyPay Card Tokenization API
  slug: dailypay-card-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-card-tokenization-api-openapi.yml
- filename: dailypay-health-api-openapi.yml
  format: yaml
  label: DailyPay Health API
  slug: dailypay-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-health-api-openapi.yml
- filename: dailypay-jobs-api-openapi.yml
  format: yaml
  label: DailyPay Jobs API
  slug: dailypay-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-jobs-api-openapi.yml
- filename: dailypay-organizations-api-openapi.yml
  format: yaml
  label: DailyPay Organizations API
  slug: dailypay-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-organizations-api-openapi.yml
- filename: dailypay-paychecks-api-openapi.yml
  format: yaml
  label: DailyPay Paychecks API
  slug: dailypay-paychecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-paychecks-api-openapi.yml
- filename: dailypay-people-api-openapi.yml
  format: yaml
  label: DailyPay People API
  slug: dailypay-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-people-api-openapi.yml
- filename: dailypay-transfers-api-openapi.yml
  format: yaml
  label: DailyPay Transfers API
  slug: dailypay-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-transfers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dailypay.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.dailypay.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 07:20:11 2026 GMT
  host: developer.dailypay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.dailypay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dailypay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DailyPay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DailyPay
provider_slug: dailypay
slug: dailypay-domain-security
source_filename: dailypay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dailypay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.dailypay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 07:20:11 2026 GMT\n  hsts: false\n- host: api.dailypay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dailypay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/security/dailypay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Payroll
- Human Resources
- Earned Wage Access
- On-Demand Pay
- Financial-Services
- Fintech
- Money Transfer
- Benefits
---
