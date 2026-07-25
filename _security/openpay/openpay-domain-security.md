---
api_specs:
- filename: openpay-bankaccounts-api-openapi.yml
  format: yaml
  label: Openpay BankAccounts API
  slug: openpay-bankaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-bankaccounts-api-openapi.yml
- filename: openpay-cards-api-openapi.yml
  format: yaml
  label: Openpay Cards API
  slug: openpay-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-cards-api-openapi.yml
- filename: openpay-charges-api-openapi.yml
  format: yaml
  label: Openpay Charges API
  slug: openpay-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-charges-api-openapi.yml
- filename: openpay-customers-api-openapi.yml
  format: yaml
  label: Openpay Customers API
  slug: openpay-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-customers-api-openapi.yml
- filename: openpay-fees-api-openapi.yml
  format: yaml
  label: Openpay Fees API
  slug: openpay-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-fees-api-openapi.yml
- filename: openpay-payouts-api-openapi.yml
  format: yaml
  label: Openpay Payouts API
  slug: openpay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-payouts-api-openapi.yml
- filename: openpay-plans-api-openapi.yml
  format: yaml
  label: Openpay Plans API
  slug: openpay-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-plans-api-openapi.yml
- filename: openpay-subscriptions-api-openapi.yml
  format: yaml
  label: Openpay Subscriptions API
  slug: openpay-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-subscriptions-api-openapi.yml
- filename: openpay-tokens-api-openapi.yml
  format: yaml
  label: Openpay Tokens API
  slug: openpay-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-tokens-api-openapi.yml
- filename: openpay-transfers-api-openapi.yml
  format: yaml
  label: Openpay Transfers API
  slug: openpay-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-transfers-api-openapi.yml
- filename: openpay-webhooks-api-openapi.yml
  format: yaml
  label: Openpay Webhooks API
  slug: openpay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/openapi/openpay-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openpay.mx
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.openpay.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: documents.openpay.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: api.openpay.mx
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Openpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openpay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Openpay
provider_slug: openpay
slug: openpay-domain-security
source_filename: openpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openpay.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documents.openpay.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openpay.mx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: openpay.mx\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpay/refs/heads/main/security/openpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Cards
- SPEI
- Subscriptions
---
