---
api_specs:
- filename: qonto-cards-api-openapi.yml
  format: yaml
  label: Qonto Cards API
  slug: qonto-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-cards-api-openapi.yml
- filename: qonto-client-invoices-api-openapi.yml
  format: yaml
  label: Qonto Client Invoices API
  slug: qonto-client-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-client-invoices-api-openapi.yml
- filename: qonto-internal-transfers-api-openapi.yml
  format: yaml
  label: Qonto Internal Transfers API
  slug: qonto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-internal-transfers-api-openapi.yml
- filename: qonto-international-transfers-api-openapi.yml
  format: yaml
  label: Qonto International Transfers API
  slug: qonto-international-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-international-transfers-api-openapi.yml
- filename: qonto-organizations-accounts-api-openapi.yml
  format: yaml
  label: Qonto Organizations & Accounts API
  slug: qonto-organizations-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-organizations-accounts-api-openapi.yml
- filename: qonto-payment-links-api-openapi.yml
  format: yaml
  label: Qonto Payment Links API
  slug: qonto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-payment-links-api-openapi.yml
- filename: qonto-sepa-direct-debit-api-openapi.yml
  format: yaml
  label: Qonto SEPA Direct Debit API
  slug: qonto-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-sepa-direct-debit-api-openapi.yml
- filename: qonto-sepa-transfers-api-openapi.yml
  format: yaml
  label: Qonto SEPA Transfers API
  slug: qonto-sepa-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-sepa-transfers-api-openapi.yml
- filename: qonto-supplier-invoices-api-openapi.yml
  format: yaml
  label: Qonto Supplier Invoices API
  slug: qonto-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-supplier-invoices-api-openapi.yml
- filename: qonto-terminals-api-openapi.yml
  format: yaml
  label: Qonto Terminals API
  slug: qonto-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-terminals-api-openapi.yml
- filename: qonto-webhooks-api-openapi.yml
  format: yaml
  label: Qonto Webhooks API
  slug: qonto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-webhooks-api-openapi.yml
- filename: qonto-oauth-api-openapi.yml
  format: yaml
  label: Qonto O Auth API
  slug: qonto-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-oauth-api-openapi.yml
- filename: qonto-transactions-and-statements-api-openapi.yml
  format: yaml
  label: Qonto Transactions and Statements API
  slug: qonto-transactions-and-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-transactions-and-statements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qonto.com
  spf: true
hosts:
- cert_expires: Apr 26 23:59:59 2027 GMT
  host: qonto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 00:47:11 2027 GMT
  host: docs.qonto.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 15:04:15 2027 GMT
  host: thirdparty.qonto.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Qonto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qonto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qonto
provider_slug: qonto
slug: qonto-domain-security
source_filename: qonto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qonto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qonto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:47:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: thirdparty.qonto.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  4 15:04:15 2027 GMT\n  hsts: null\ndomains:\n- domain: qonto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/security/qonto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Banking
- Neobank
- Fintech
- Payments
- SEPA
- Open Banking
- EUR
- Europe
---
