---
api_specs:
- filename: plug-3ds2-malga-api-openapi.yml
  format: yaml
  label: Malga 3DS2 Malga API
  slug: plug-3ds2-malga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-3ds2-malga-api-openapi.yml
- filename: plug-cards-api-openapi.yml
  format: yaml
  label: Malga Cards API
  slug: plug-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-cards-api-openapi.yml
- filename: plug-charges-api-openapi.yml
  format: yaml
  label: Malga Charges API
  slug: plug-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-charges-api-openapi.yml
- filename: plug-client-token-api-openapi.yml
  format: yaml
  label: Malga Client-token API
  slug: plug-client-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-client-token-api-openapi.yml
- filename: plug-customers-api-openapi.yml
  format: yaml
  label: Malga Customers API
  slug: plug-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-customers-api-openapi.yml
- filename: plug-flows-api-openapi.yml
  format: yaml
  label: Malga Flows API
  slug: plug-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-flows-api-openapi.yml
- filename: plug-merchants-api-openapi.yml
  format: yaml
  label: Malga Merchants API
  slug: plug-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-merchants-api-openapi.yml
- filename: plug-payouts-api-openapi.yml
  format: yaml
  label: Malga Payouts API
  slug: plug-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-payouts-api-openapi.yml
- filename: plug-prepayment-api-openapi.yml
  format: yaml
  label: Malga Prepayment API
  slug: plug-prepayment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-prepayment-api-openapi.yml
- filename: plug-providers-api-openapi.yml
  format: yaml
  label: Malga Providers API
  slug: plug-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-providers-api-openapi.yml
- filename: plug-seller-documents-api-openapi.yml
  format: yaml
  label: Malga Seller Documents API
  slug: plug-seller-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-seller-documents-api-openapi.yml
- filename: plug-sellers-api-openapi.yml
  format: yaml
  label: Malga Sellers API
  slug: plug-sellers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-sellers-api-openapi.yml
- filename: plug-sessions-api-openapi.yml
  format: yaml
  label: Malga Sessions API
  slug: plug-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-sessions-api-openapi.yml
- filename: plug-settings-api-openapi.yml
  format: yaml
  label: Malga Settings API
  slug: plug-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-settings-api-openapi.yml
- filename: plug-subscriptions-api-openapi.yml
  format: yaml
  label: Malga Subscriptions API
  slug: plug-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-subscriptions-api-openapi.yml
- filename: plug-tokens-api-openapi.yml
  format: yaml
  label: Malga Tokens API
  slug: plug-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-tokens-api-openapi.yml
- filename: plug-vendors-api-openapi.yml
  format: yaml
  label: Malga Vendors API
  slug: plug-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-vendors-api-openapi.yml
- filename: plug-webhooks-api-openapi.yml
  format: yaml
  label: Malga Webhooks API
  slug: plug-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/openapi/plug-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: malga.io
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: malga.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 16:56:13 2026 GMT
  host: docs.malga.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.malga.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Malga, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Malga
provider_slug: plug
slug: plug-domain-security
source_filename: plug-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: malga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\n- host: docs.malga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:56:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.malga.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: malga.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plug/refs/heads/main/security/plug-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Orchestration
- Payment Gateway
- Fintech
- Pix
- Tokenization
- Subscriptions
- Brazil
---
