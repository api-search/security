---
api_specs:
- filename: lago-add-ons-api-openapi.yml
  format: yaml
  label: Lago Add_ons API
  slug: lago-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-add-ons-api-openapi.yml
- filename: lago-analytics-api-openapi.yml
  format: yaml
  label: Lago Analytics API
  slug: lago-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-analytics-api-openapi.yml
- filename: lago-billable-metrics-api-openapi.yml
  format: yaml
  label: Lago Billable_metrics API
  slug: lago-billable-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-billable-metrics-api-openapi.yml
- filename: lago-coupons-api-openapi.yml
  format: yaml
  label: Lago Coupons API
  slug: lago-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-coupons-api-openapi.yml
- filename: lago-credit-notes-api-openapi.yml
  format: yaml
  label: Lago Credit_notes API
  slug: lago-credit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-credit-notes-api-openapi.yml
- filename: lago-customers-api-openapi.yml
  format: yaml
  label: Lago Customers API
  slug: lago-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-customers-api-openapi.yml
- filename: lago-events-api-openapi.yml
  format: yaml
  label: Lago Events API
  slug: lago-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-events-api-openapi.yml
- filename: lago-fees-api-openapi.yml
  format: yaml
  label: Lago Fees API
  slug: lago-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-fees-api-openapi.yml
- filename: lago-invoices-api-openapi.yml
  format: yaml
  label: Lago Invoices API
  slug: lago-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-invoices-api-openapi.yml
- filename: lago-organizations-api-openapi.yml
  format: yaml
  label: Lago Organizations API
  slug: lago-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-organizations-api-openapi.yml
- filename: lago-payment-requests-api-openapi.yml
  format: yaml
  label: Lago Payment_requests API
  slug: lago-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-payment-requests-api-openapi.yml
- filename: lago-plans-api-openapi.yml
  format: yaml
  label: Lago Plans API
  slug: lago-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-plans-api-openapi.yml
- filename: lago-subscriptions-api-openapi.yml
  format: yaml
  label: Lago Subscriptions API
  slug: lago-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-subscriptions-api-openapi.yml
- filename: lago-taxes-api-openapi.yml
  format: yaml
  label: Lago Taxes API
  slug: lago-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-taxes-api-openapi.yml
- filename: lago-wallets-api-openapi.yml
  format: yaml
  label: Lago Wallets API
  slug: lago-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-wallets-api-openapi.yml
- filename: lago-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Lago Webhook_endpoints API
  slug: lago-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-webhook-endpoints-api-openapi.yml
- filename: lago-webhooks-api-openapi.yml
  format: yaml
  label: Lago Webhooks API
  slug: lago-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/openapi/lago-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getlago.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: getlago.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 20:40:11 2026 GMT
  host: api.getlago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 20:11:05 2026 GMT
  host: api.eu.getlago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lago, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lago
provider_slug: lago
slug: lago-domain-security
source_filename: lago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getlago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: api.getlago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 20:40:11 2026 GMT\n  hsts: null\n- host: api.eu.getlago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 20:11:05 2026 GMT\n  hsts: null\ndomains:\n- domain: getlago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lago/refs/heads/main/security/lago-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Billing
- Metering
- Open Source
- Usage-Based
---
