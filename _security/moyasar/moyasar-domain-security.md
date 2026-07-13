---
api_specs:
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Payments API
  slug: moyasar-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Invoices API
  slug: moyasar-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Tokens API
  slug: moyasar-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Webhooks API
  slug: moyasar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
- filename: moyasar-openapi.yml
  format: yaml
  label: Moyasar Payouts API
  slug: moyasar-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/openapi/moyasar-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dnssec: false
  domain: moyasar.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Dec  5 08:16:03 2026 GMT
  host: moyasar.com
  hsts: false
  https: true
  note: Apex returned HTTP/2 200 without a Strict-Transport-Security header at probe time.
  tls_version: TLSv1.3
- cert_expires: Dec  5 08:16:03 2026 GMT
  host: api.moyasar.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 17:46:27 2026 GMT
  host: docs.moyasar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moyasar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moyasar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moyasar
provider_slug: moyasar
slug: moyasar-domain-security
source_filename: moyasar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moyasar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 08:16:03 2026 GMT\n  hsts: false\n  note: Apex returned HTTP/2 200 without a Strict-Transport-Security header at probe time.\n- host: api.moyasar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 08:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: docs.moyasar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:46:27 2026 GMT\n  hsts: false\ndomains:\n- domain: moyasar.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 100\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moyasar/refs/heads/main/security/moyasar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Saudi Arabia
- MENA
- mada
- Cards
- Apple Pay
- STC Pay
- Invoices
- Fintech
---
