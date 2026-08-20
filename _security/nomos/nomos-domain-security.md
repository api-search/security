---
api_specs:
- filename: nomos-authentication-api-openapi.yml
  format: yaml
  label: Nomos Authentication API
  slug: nomos-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-authentication-api-openapi.yml
- filename: nomos-customers-api-openapi.yml
  format: yaml
  label: Nomos Customers API
  slug: nomos-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-customers-api-openapi.yml
- filename: nomos-events-api-openapi.yml
  format: yaml
  label: Nomos Events API
  slug: nomos-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-events-api-openapi.yml
- filename: nomos-grid-fee-reductions-api-openapi.yml
  format: yaml
  label: Nomos Grid Fee Reductions API
  slug: nomos-grid-fee-reductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-grid-fee-reductions-api-openapi.yml
- filename: nomos-invoices-api-openapi.yml
  format: yaml
  label: Nomos Invoices API
  slug: nomos-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-invoices-api-openapi.yml
- filename: nomos-leads-api-openapi.yml
  format: yaml
  label: Nomos Leads API
  slug: nomos-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-leads-api-openapi.yml
- filename: nomos-market-partners-api-openapi.yml
  format: yaml
  label: Nomos Market Partners API
  slug: nomos-market-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-market-partners-api-openapi.yml
- filename: nomos-plans-api-openapi.yml
  format: yaml
  label: Nomos Plans API
  slug: nomos-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-plans-api-openapi.yml
- filename: nomos-prices-api-openapi.yml
  format: yaml
  label: Nomos Prices API
  slug: nomos-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-prices-api-openapi.yml
- filename: nomos-smart-meter-orders-api-openapi.yml
  format: yaml
  label: Nomos Smart Meter Orders API
  slug: nomos-smart-meter-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-smart-meter-orders-api-openapi.yml
- filename: nomos-subscriptions-api-openapi.yml
  format: yaml
  label: Nomos Subscriptions API
  slug: nomos-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-subscriptions-api-openapi.yml
- filename: nomos-usage-api-openapi.yml
  format: yaml
  label: Nomos Usage API
  slug: nomos-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/openapi/nomos-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomos.energy
  spf: true
hosts:
- cert_expires: Oct  5 23:25:28 2026 GMT
  host: api.nomos.energy
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nomos
provider_slug: nomos
slug: nomos-domain-security
source_filename: nomos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nomos.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:25:28 2026 GMT\n  hsts: false\ndomains:\n- domain: nomos.energy\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomos/refs/heads/main/security/nomos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Electricity
- Utilities
- Embedded Finance
- Dynamic Pricing
- Billing
- Metering
- Smart Meter
- Germany
- Authentication
- Webhook
---
