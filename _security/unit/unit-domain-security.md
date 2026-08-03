---
api_specs:
- filename: unit-applications-openapi.json
  format: json
  label: Unit Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-applications-openapi.json
- filename: unit-customers-openapi.json
  format: json
  label: Unit Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-customers-openapi.json
- filename: unit-accounts-openapi.json
  format: json
  label: Unit Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-accounts-openapi.json
- filename: unit-cards-openapi.json
  format: json
  label: Unit Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-cards-openapi.json
- filename: unit-payments-openapi.json
  format: json
  label: Unit Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-payments-openapi.json
- filename: unit-checks-openapi.json
  format: json
  label: Unit Checks API
  slug: checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-checks-openapi.json
- filename: unit-authorizations-openapi.json
  format: json
  label: Unit Card Authorizations API
  slug: authorizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-authorizations-openapi.json
- filename: unit-disputes-openapi.json
  format: json
  label: Unit Disputes API
  slug: disputes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-disputes-openapi.json
- filename: unit-transactions-openapi.json
  format: json
  label: Unit Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-transactions-openapi.json
- filename: unit-statements-openapi.json
  format: json
  label: Unit Statements API
  slug: statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-statements-openapi.json
- filename: unit-tax-forms-openapi.json
  format: json
  label: Unit Tax Forms API
  slug: tax-forms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-tax-forms-openapi.json
- filename: unit-fees-rewards-openapi.json
  format: json
  label: Unit Fees and Rewards API
  slug: fees-rewards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-fees-rewards-openapi.json
- filename: unit-credit-openapi.json
  format: json
  label: Unit Credit and Repayments API
  slug: credit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-credit-openapi.json
- filename: unit-stop-payments-openapi.json
  format: json
  label: Unit Stop Payments API
  slug: stop-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-stop-payments-openapi.json
- filename: unit-webhooks-openapi.json
  format: json
  label: Unit Webhooks and Events API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-webhooks-openapi.json
- filename: unit-sandbox-openapi.json
  format: json
  label: Unit Sandbox and Reference API
  slug: sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-sandbox-openapi.json
- filename: unit-openapi-source.json
  format: json
  label: Unit OpenAPI specifications
  slug: unit-openapi-source
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-openapi-source.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unit.co
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.unit.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.unit.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unit
provider_slug: unit
slug: unit-domain-security
source_filename: unit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.unit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: unit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/security/unit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
- United States
- Embedded Finance
- Deposit Accounts
- Open Finance
---
