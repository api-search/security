---
api_specs:
- filename: plaid-plaid-api-openapi.yml
  format: yaml
  label: Plaid API
  slug: plaid-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-plaid-api-openapi.yml
- filename: plaid-account-information-api-openapi.yml
  format: yaml
  label: Plaid Account Information API
  slug: plaid-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-information-api-openapi.yml
- filename: plaid-account-statements-api-openapi.yml
  format: yaml
  label: Plaid Account Statements API
  slug: plaid-account-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-statements-api-openapi.yml
- filename: plaid-account-transactions-api-openapi.yml
  format: yaml
  label: Plaid Account Transactions API
  slug: plaid-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-transactions-api-openapi.yml
- filename: plaid-asset-transfer-networks-information-api-openapi.yml
  format: yaml
  label: Plaid Asset Transfer Networks Information API
  slug: plaid-asset-transfer-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-asset-transfer-networks-information-api-openapi.yml
- filename: plaid-payment-networks-information-api-openapi.yml
  format: yaml
  label: Plaid Payment Networks Information API
  slug: plaid-payment-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-payment-networks-information-api-openapi.yml
- filename: plaid-personal-information-api-openapi.yml
  format: yaml
  label: Plaid Personal Information API
  slug: plaid-personal-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-personal-information-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plaid.com
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
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
- host: development.plaid.com
  https: false
hosts_probed: 3
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
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.plaid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\n- host: development.plaid.com\n  https: false\ndomains:\n- domain: plaid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/security/plaid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Fintech
- Open Banking
- Bank Accounts
- Data Aggregation
- Payments
- United States
---
