---
api_specs:
- filename: upbit-exchange-account-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Account API
  slug: upbit-exchange-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-account-api-openapi.yml
- filename: upbit-exchange-deposits-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Deposits API
  slug: upbit-exchange-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-deposits-api-openapi.yml
- filename: upbit-exchange-orders-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Orders API
  slug: upbit-exchange-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-orders-api-openapi.yml
- filename: upbit-exchange-service-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Service API
  slug: upbit-exchange-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-service-api-openapi.yml
- filename: upbit-exchange-travel-rule-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Travel Rule API
  slug: upbit-exchange-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-travel-rule-api-openapi.yml
- filename: upbit-exchange-withdrawals-api-openapi.yml
  format: yaml
  label: Upbit Exchange - Withdrawals API
  slug: upbit-exchange-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-exchange-withdrawals-api-openapi.yml
- filename: upbit-quotation-api-openapi.yml
  format: yaml
  label: Upbit Quotation API
  slug: upbit-quotation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/openapi/upbit-quotation-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upbit.com
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: upbit.com
  hsts: true
  hsts_max_age: 631139040
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:45:36 2026 GMT
  host: global-docs.upbit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.upbit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upbit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Upbit
provider_slug: upbit
slug: upbit-domain-security
source_filename: upbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631139040\n- host: global-docs.upbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:45:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upbit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upbit/refs/heads/main/security/upbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Exchange
- Market Data
- Orders
- Trading
- WebSocket
---
