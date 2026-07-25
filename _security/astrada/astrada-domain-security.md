---
api_specs:
- filename: astrada-bank-accounts-api-openapi.yml
  format: yaml
  label: Astrada bank-accounts API
  slug: astrada-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-bank-accounts-api-openapi.yml
- filename: astrada-bank-links-api-openapi.yml
  format: yaml
  label: Astrada bank-links API
  slug: astrada-bank-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-bank-links-api-openapi.yml
- filename: astrada-bank-subscriptions-api-openapi.yml
  format: yaml
  label: Astrada bank-subscriptions API
  slug: astrada-bank-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-bank-subscriptions-api-openapi.yml
- filename: astrada-bank-transactions-api-openapi.yml
  format: yaml
  label: Astrada bank-transactions API
  slug: astrada-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-bank-transactions-api-openapi.yml
- filename: astrada-bin-lookup-api-openapi.yml
  format: yaml
  label: Astrada bin-lookup API
  slug: astrada-bin-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-bin-lookup-api-openapi.yml
- filename: astrada-card-api-openapi.yml
  format: yaml
  label: Astrada card API
  slug: astrada-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-card-api-openapi.yml
- filename: astrada-card-subscription-api-openapi.yml
  format: yaml
  label: Astrada card-subscription API
  slug: astrada-card-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-card-subscription-api-openapi.yml
- filename: astrada-card-verification-api-openapi.yml
  format: yaml
  label: Astrada card-verification API
  slug: astrada-card-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-card-verification-api-openapi.yml
- filename: astrada-enrollment-methods-api-openapi.yml
  format: yaml
  label: Astrada enrollment-methods API
  slug: astrada-enrollment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-enrollment-methods-api-openapi.yml
- filename: astrada-network-bulk-feeds-api-openapi.yml
  format: yaml
  label: Astrada network-bulk-feeds API
  slug: astrada-network-bulk-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-network-bulk-feeds-api-openapi.yml
- filename: astrada-subaccounts-api-openapi.yml
  format: yaml
  label: Astrada subaccounts API
  slug: astrada-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-subaccounts-api-openapi.yml
- filename: astrada-transaction-matches-api-openapi.yml
  format: yaml
  label: Astrada transaction-matches API
  slug: astrada-transaction-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-transaction-matches-api-openapi.yml
- filename: astrada-transaction-messages-api-openapi.yml
  format: yaml
  label: Astrada transaction-messages API
  slug: astrada-transaction-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-transaction-messages-api-openapi.yml
- filename: astrada-transactions-api-openapi.yml
  format: yaml
  label: Astrada transactions API
  slug: astrada-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-transactions-api-openapi.yml
- filename: astrada-webhooks-api-openapi.yml
  format: yaml
  label: Astrada webhooks API
  slug: astrada-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/openapi/astrada-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astrada.co
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: astrada.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astrada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Astrada
provider_slug: astrada
slug: astrada-domain-security
source_filename: astrada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astrada.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: astrada.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrada/refs/heads/main/security/astrada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Card Data
- Transaction Data
- Reconciliation
- Expense Management
- Data Infrastructure
---
