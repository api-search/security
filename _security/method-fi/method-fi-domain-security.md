---
api_specs:
- filename: method-fi-accounts-api-openapi.yml
  format: yaml
  label: Method Financial Accounts API
  slug: method-fi-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-accounts-api-openapi.yml
- filename: method-fi-connect-api-openapi.yml
  format: yaml
  label: Method Financial Connect API
  slug: method-fi-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-connect-api-openapi.yml
- filename: method-fi-entities-api-openapi.yml
  format: yaml
  label: Method Financial Entities API
  slug: method-fi-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-entities-api-openapi.yml
- filename: method-fi-merchants-api-openapi.yml
  format: yaml
  label: Method Financial Merchants API
  slug: method-fi-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-merchants-api-openapi.yml
- filename: method-fi-payments-api-openapi.yml
  format: yaml
  label: Method Financial Payments API
  slug: method-fi-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-payments-api-openapi.yml
- filename: method-fi-transactions-api-openapi.yml
  format: yaml
  label: Method Financial Transactions API
  slug: method-fi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-transactions-api-openapi.yml
- filename: method-fi-webhooks-api-openapi.yml
  format: yaml
  label: Method Financial Webhooks API
  slug: method-fi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/openapi/method-fi-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: methodfi.com
  spf: true
hosts:
- cert_expires: Sep 27 00:11:29 2026 GMT
  host: methodfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 01:04:02 2026 GMT
  host: docs.methodfi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 07:23:50 2026 GMT
  host: production.methodfi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Method Fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Method Financial, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Method Financial
provider_slug: method-fi
slug: method-fi-domain-security
source_filename: method-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: methodfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.methodfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:04:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.methodfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:23:50 2026 GMT\n  hsts: null\ndomains:\n- domain: methodfi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/method-fi/refs/heads/main/security/method-fi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- Payments
- Liabilities
- Debt
- Embedded Finance
---
