---
api_specs:
- filename: orb-billing-alerts-api-openapi.yml
  format: yaml
  label: Orb Alerts API
  slug: orb-billing-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-alerts-api-openapi.yml
- filename: orb-billing-coupons-api-openapi.yml
  format: yaml
  label: Orb Coupons API
  slug: orb-billing-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-coupons-api-openapi.yml
- filename: orb-billing-credits-api-openapi.yml
  format: yaml
  label: Orb Credits API
  slug: orb-billing-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-credits-api-openapi.yml
- filename: orb-billing-customers-api-openapi.yml
  format: yaml
  label: Orb Customers API
  slug: orb-billing-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-customers-api-openapi.yml
- filename: orb-billing-events-api-openapi.yml
  format: yaml
  label: Orb Events API
  slug: orb-billing-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-events-api-openapi.yml
- filename: orb-billing-invoices-api-openapi.yml
  format: yaml
  label: Orb Invoices API
  slug: orb-billing-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-invoices-api-openapi.yml
- filename: orb-billing-items-api-openapi.yml
  format: yaml
  label: Orb Items API
  slug: orb-billing-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-items-api-openapi.yml
- filename: orb-billing-metrics-api-openapi.yml
  format: yaml
  label: Orb Metrics API
  slug: orb-billing-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-metrics-api-openapi.yml
- filename: orb-billing-plans-api-openapi.yml
  format: yaml
  label: Orb Plans API
  slug: orb-billing-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-plans-api-openapi.yml
- filename: orb-billing-prices-api-openapi.yml
  format: yaml
  label: Orb Prices API
  slug: orb-billing-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-prices-api-openapi.yml
- filename: orb-billing-subscriptions-api-openapi.yml
  format: yaml
  label: Orb Subscriptions API
  slug: orb-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: withorb.com
  spf: true
hosts:
- cert_expires: Oct  6 16:29:06 2026 GMT
  host: www.withorb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 14:31:11 2026 GMT
  host: docs.withorb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.withorb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orb Billing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orb, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orb
provider_slug: orb-billing
slug: orb-billing-domain-security
source_filename: orb-billing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withorb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:29:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.withorb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 14:31:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.withorb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: withorb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/security/orb-billing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Usage-Based Billing
- Metering
- Subscriptions
- Invoicing
- FinOps
---
