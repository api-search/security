---
api_specs:
- filename: spade-card-enrichment-api-openapi.yml
  format: yaml
  label: Spade Card Enrichment API
  slug: spade-card-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-card-enrichment-api-openapi.yml
- filename: spade-category-action-triggers-api-openapi.yml
  format: yaml
  label: Spade Category Action Triggers API
  slug: spade-category-action-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-category-action-triggers-api-openapi.yml
- filename: spade-category-personalization-api-openapi.yml
  format: yaml
  label: Spade Category Personalization API
  slug: spade-category-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-category-personalization-api-openapi.yml
- filename: spade-feedback-and-reporting-api-openapi.yml
  format: yaml
  label: Spade Feedback and Reporting API
  slug: spade-feedback-and-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-feedback-and-reporting-api-openapi.yml
- filename: spade-merchant-action-triggers-api-openapi.yml
  format: yaml
  label: Spade Merchant Action Triggers API
  slug: spade-merchant-action-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-merchant-action-triggers-api-openapi.yml
- filename: spade-merchant-search-api-openapi.yml
  format: yaml
  label: Spade Merchant Search API
  slug: spade-merchant-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-merchant-search-api-openapi.yml
- filename: spade-transfer-enrichment-api-openapi.yml
  format: yaml
  label: Spade Transfer Enrichment API
  slug: spade-transfer-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-transfer-enrichment-api-openapi.yml
- filename: spade-universal-enrichment-api-openapi.yml
  format: yaml
  label: Spade Universal Enrichment API
  slug: spade-universal-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/openapi/spade-universal-enrichment-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spade.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: east.sandbox.spade.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: east.api.spade.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: west.sandbox.spade.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spade
provider_slug: spade
slug: spade-domain-security
source_filename: spade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: east.sandbox.spade.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: east.api.spade.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: west.sandbox.spade.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: spade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spade/refs/heads/main/security/spade-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Financial Services
- Transaction Enrichment
- Merchant Intelligence
- Payments
- Data Enrichment
- Fraud and Risk
- Fintech
---
