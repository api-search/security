---
api_specs:
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Connect API
  slug: bud-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud First-Party Ingestion API
  slug: bud-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customers Platform API
  slug: bud-customers-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Data API
  slug: bud-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Enrichment API
  slug: bud-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Financial Insights API
  slug: bud-financial-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Intelligent Search API
  slug: bud-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Affordability and Assess API
  slug: bud-affordability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Customer Characteristics API
  slug: bud-characteristics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Goals and Budgets API
  slug: bud-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Payments API
  slug: bud-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
- filename: bud-platform-openapi.yml
  format: yaml
  label: Bud Embedded Widgets API
  slug: bud-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/openapi/bud-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bud.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thisisbud.com
  spf: true
hosts:
- host: bud.co
  https: false
- cert_expires: Oct  2 12:11:34 2026 GMT
  host: docs.thisisbud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 21 08:38:18 2026 GMT
  host: api-sandbox.thisisbud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bud Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bud Financial, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bud Financial
provider_slug: bud-co
slug: bud-co-domain-security
source_filename: bud-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bud.co\n  https: false\n- host: docs.thisisbud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:11:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.thisisbud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 08:38:18 2026 GMT\n  hsts: null\ndomains:\n- domain: bud.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thisisbud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bud-co/refs/heads/main/security/bud-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Banking
- Transaction Enrichment
- Categorization
- Affordability
- Payments
- AISP
- PISP
- Financial Data
- FinTech
- UK
- AI
- Machine Learning
---
