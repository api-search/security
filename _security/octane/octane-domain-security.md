---
api_specs:
- filename: octane-admin-api-openapi.yml
  format: yaml
  label: Octane Admin API
  slug: octane-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-admin-api-openapi.yml
- filename: octane-avalara-api-openapi.yml
  format: yaml
  label: Octane Avalara API
  slug: octane-avalara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-avalara-api-openapi.yml
- filename: octane-billing-settings-api-openapi.yml
  format: yaml
  label: Octane Billing Settings API
  slug: octane-billing-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-billing-settings-api-openapi.yml
- filename: octane-coupons-api-openapi.yml
  format: yaml
  label: Octane Coupons API
  slug: octane-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-coupons-api-openapi.yml
- filename: octane-credits-api-openapi.yml
  format: yaml
  label: Octane Credits API
  slug: octane-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-credits-api-openapi.yml
- filename: octane-customer-portal-api-openapi.yml
  format: yaml
  label: Octane Customer Portal API
  slug: octane-customer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-customer-portal-api-openapi.yml
- filename: octane-customers-api-openapi.yml
  format: yaml
  label: Octane Customers API
  slug: octane-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-customers-api-openapi.yml
- filename: octane-features-api-openapi.yml
  format: yaml
  label: Octane Features API
  slug: octane-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-features-api-openapi.yml
- filename: octane-invoices-api-openapi.yml
  format: yaml
  label: Octane Invoices API
  slug: octane-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-invoices-api-openapi.yml
- filename: octane-live-measurements-api-openapi.yml
  format: yaml
  label: Octane Live Measurements API
  slug: octane-live-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-live-measurements-api-openapi.yml
- filename: octane-measurements-api-openapi.yml
  format: yaml
  label: Octane Measurements API
  slug: octane-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-measurements-api-openapi.yml
- filename: octane-meters-api-openapi.yml
  format: yaml
  label: Octane Meters API
  slug: octane-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-meters-api-openapi.yml
- filename: octane-price-plans-api-openapi.yml
  format: yaml
  label: Octane Price Plans API
  slug: octane-price-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-price-plans-api-openapi.yml
- filename: octane-refunds-api-openapi.yml
  format: yaml
  label: Octane Refunds API
  slug: octane-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-refunds-api-openapi.yml
- filename: octane-revenue-recognition-api-openapi.yml
  format: yaml
  label: Octane Revenue Recognition API
  slug: octane-revenue-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-revenue-recognition-api-openapi.yml
- filename: octane-subscriptions-api-openapi.yml
  format: yaml
  label: Octane Subscriptions API
  slug: octane-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-subscriptions-api-openapi.yml
- filename: octane-webhooks-api-openapi.yml
  format: yaml
  label: Octane Webhooks API
  slug: octane-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/openapi/octane-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getoctane.io
  spf: true
hosts:
- cert_expires: Oct  8 13:02:21 2026 GMT
  host: www.getoctane.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: docs.getoctane.io
  https: false
- host: api.getoctane.io
  https: false
kind: domain-security
layout: security
method: probed
name: Octane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octane, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Octane
provider_slug: octane
slug: octane-domain-security
source_filename: octane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getoctane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:02:21 2026 GMT\n  hsts: false\n- host: docs.getoctane.io\n  https: false\n- host: api.getoctane.io\n  https: false\ndomains:\n- domain: getoctane.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octane/refs/heads/main/security/octane-domain-security.yml
summary_line: TLSv1.3
tags:
- Usage-Based Billing
- Metered Billing
- Pricing Plans
- SaaS Monetization
- FinTech
- Payments
- Usage Tracking
- Meters
- Entitlements
---
