---
api_specs:
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Customers API
  slug: orb-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Plans API
  slug: orb-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Subscriptions API
  slug: orb-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Events & Ingestion API
  slug: orb-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Metrics API
  slug: orb-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Invoices API
  slug: orb-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Credits & Ledger API
  slug: orb-credits-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Prices & Items API
  slug: orb-prices-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Alerts & Coupons API
  slug: orb-alerts-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
- filename: orb-billing-openapi.yml
  format: yaml
  label: Orb Webhooks API
  slug: orb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orb-billing/refs/heads/main/openapi/orb-billing-openapi.yml
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
