---
api_specs:
- filename: ebanx-pay-in-direct-api-openapi.yml
  format: yaml
  label: EBANX Pay-in Direct API
  slug: ebanx-pay-in-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-pay-in-direct-api-openapi.yml
- filename: ebanx-payment-page-api-openapi.yml
  format: yaml
  label: EBANX Payment Page API
  slug: ebanx-payment-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-payment-page-api-openapi.yml
- filename: ebanx-tokenization-api-openapi.yml
  format: yaml
  label: EBANX Tokenization API
  slug: ebanx-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-tokenization-api-openapi.yml
- filename: ebanx-fx-api-openapi.yml
  format: yaml
  label: EBANX FX API
  slug: ebanx-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-fx-api-openapi.yml
- filename: ebanx-payout-api-openapi.yml
  format: yaml
  label: EBANX Payout API
  slug: ebanx-payout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/openapi/ebanx-payout-api-openapi.yml
- filename: ebanx-notifications-asyncapi.yml
  format: yaml
  label: EBANX Payment Notifications
  slug: ebanx-notifications
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/asyncapi/ebanx-notifications-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ebanx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ebanxpay.com
  spf: true
hosts:
- cert_expires: Aug 22 02:16:20 2026 GMT
  host: docs.ebanx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:44:55 2026 GMT
  host: api.ebanxpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:44:55 2026 GMT
  host: sandbox.ebanxpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ebanx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EBANX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EBANX
provider_slug: ebanx
slug: ebanx-domain-security
source_filename: ebanx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ebanx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:16:20 2026 GMT\n  hsts: false\n- host: api.ebanxpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:44:55 2026 GMT\n  hsts: null\n- host: sandbox.ebanxpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:44:55 2026 GMT\n  hsts: null\ndomains:\n- domain: ebanx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ebanxpay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebanx/refs/heads/main/security/ebanx-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Payments
- Pay-in
- Payouts
- Foreign Exchange
- Tokenization
- LATAM
- Emerging Markets
- Pix
- Boleto
- OXXO
- SPEI
- PSE
- Cross-Border
- Webhooks
---
