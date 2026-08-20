---
api_specs:
- filename: chase-rewards-balance-api-openapi.yml
  format: yaml
  label: Chase Rewards Balance API
  slug: rewards-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-rewards-balance-api-openapi.yml
- filename: chase-accounts-api-openapi.yml
  format: yaml
  label: Chase Accounts API
  slug: chase-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-accounts-api-openapi.yml
- filename: chase-consents-api-openapi.yml
  format: yaml
  label: Chase Consents API
  slug: chase-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-consents-api-openapi.yml
- filename: chase-customers-api-openapi.yml
  format: yaml
  label: Chase Customers API
  slug: chase-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-customers-api-openapi.yml
- filename: chase-enrollments-api-openapi.yml
  format: yaml
  label: Chase Enrollments API
  slug: chase-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-enrollments-api-openapi.yml
- filename: chase-merchants-api-openapi.yml
  format: yaml
  label: Chase Merchants API
  slug: chase-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-merchants-api-openapi.yml
- filename: chase-orders-api-openapi.yml
  format: yaml
  label: Chase Orders API
  slug: chase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-orders-api-openapi.yml
- filename: chase-refunds-api-openapi.yml
  format: yaml
  label: Chase Refunds API
  slug: chase-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-refunds-api-openapi.yml
- filename: chase-statements-api-openapi.yml
  format: yaml
  label: Chase Statements API
  slug: chase-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-statements-api-openapi.yml
- filename: chase-tax-forms-api-openapi.yml
  format: yaml
  label: Chase Tax Forms API
  slug: chase-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-tax-forms-api-openapi.yml
- filename: chase-transactions-api-openapi.yml
  format: yaml
  label: Chase Transactions API
  slug: chase-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/openapi/chase-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chase.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.chase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: developer.chase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.chase.com
  https: false
kind: domain-security
layout: security
method: probed
name: Chase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chase, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chase
provider_slug: chase
slug: chase-domain-security
source_filename: chase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.chase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: null\n- host: api.chase.com\n  https: false\ndomains:\n- domain: chase.com\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/security/chase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Account Aggregation
- Banking
- Consent
- Credit Cards
- FDX
- Financial-Services
- Loyalty
- Open Banking
- Pay with Points
- Rewards
---
