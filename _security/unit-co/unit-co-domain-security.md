---
api_specs:
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Applications API
  slug: unit-co-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Customers API
  slug: unit-co-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Accounts API
  slug: unit-co-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Cards API
  slug: unit-co-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Card Authorizations API
  slug: unit-co-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Payments API
  slug: unit-co-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Counterparties API
  slug: unit-co-counterparties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Checks API
  slug: unit-co-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Transactions API
  slug: unit-co-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Statements and Tax Forms API
  slug: unit-co-statements-tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Events and Webhooks API
  slug: unit-co-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Risk and Fraud Prevention API
  slug: unit-co-risk-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Credit and Repayments API
  slug: unit-co-credit-repayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit Fees and Rewards API
  slug: unit-co-fees-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
- filename: unit-co-openapi.yml
  format: yaml
  label: Unit API Tokens API
  slug: unit-co-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/openapi/unit-co-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unit.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unit.sh
  spf: false
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.unit.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.s.unit.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 14:54:05 2026 GMT
  host: docs.unit.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unit Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unit
provider_slug: unit-co
slug: unit-co-domain-security
source_filename: unit-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.s.unit.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.unit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 14:54:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: unit.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit-co/refs/heads/main/security/unit-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
- Lending
- JSON:API
---
