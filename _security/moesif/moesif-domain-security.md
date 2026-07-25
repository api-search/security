---
api_specs:
- filename: moesif-applications-api-openapi.yml
  format: yaml
  label: Moesif Applications API
  slug: moesif-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-applications-api-openapi.yml
- filename: moesif-balance-transactions-api-openapi.yml
  format: yaml
  label: Moesif Balance Transactions API
  slug: moesif-balance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-balance-transactions-api-openapi.yml
- filename: moesif-billing-meters-api-openapi.yml
  format: yaml
  label: Moesif Billing Meters API
  slug: moesif-billing-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-billing-meters-api-openapi.yml
- filename: moesif-billing-reports-api-openapi.yml
  format: yaml
  label: Moesif Billing Reports API
  slug: moesif-billing-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-billing-reports-api-openapi.yml
- filename: moesif-cohorts-api-openapi.yml
  format: yaml
  label: Moesif Cohorts API
  slug: moesif-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-cohorts-api-openapi.yml
- filename: moesif-companies-api-openapi.yml
  format: yaml
  label: Moesif Companies API
  slug: moesif-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-companies-api-openapi.yml
- filename: moesif-dashboards-api-openapi.yml
  format: yaml
  label: Moesif Dashboards API
  slug: moesif-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-dashboards-api-openapi.yml
- filename: moesif-email-templates-api-openapi.yml
  format: yaml
  label: Moesif Email Templates API
  slug: moesif-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-email-templates-api-openapi.yml
- filename: moesif-governance-rules-api-openapi.yml
  format: yaml
  label: Moesif Governance Rules API
  slug: moesif-governance-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-governance-rules-api-openapi.yml
- filename: moesif-metrics-api-openapi.yml
  format: yaml
  label: Moesif Metrics API
  slug: moesif-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-metrics-api-openapi.yml
- filename: moesif-product-catalog-api-openapi.yml
  format: yaml
  label: Moesif Product Catalog API
  slug: moesif-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-product-catalog-api-openapi.yml
- filename: moesif-properties-api-openapi.yml
  format: yaml
  label: Moesif Properties API
  slug: moesif-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-properties-api-openapi.yml
- filename: moesif-subscriptions-api-openapi.yml
  format: yaml
  label: Moesif Subscriptions API
  slug: moesif-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-subscriptions-api-openapi.yml
- filename: moesif-users-api-openapi.yml
  format: yaml
  label: Moesif Users API
  slug: moesif-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-users-api-openapi.yml
- filename: moesif-workspaces-api-openapi.yml
  format: yaml
  label: Moesif Workspaces API
  slug: moesif-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moesif.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: moesif.net
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.moesif.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: api.moesif.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.moesif.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moesif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moesif, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moesif
provider_slug: moesif
slug: moesif-domain-security
source_filename: moesif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moesif.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moesif.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: api.moesif.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: moesif.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: moesif.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/security/moesif-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Monitoring
- Monetization
- Governance
- Observability
- Billing
- AI Agents
- LLM Analytics
- OpenTelemetry
- Developer Portal
- Platform
- Insights
---
